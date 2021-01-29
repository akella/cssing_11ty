---
title: "Как сжимать CSS"
date: "2005-04-07"
categories: 
  - "perevod"
  - "useful"
---

Иногда на больших сайтах размер CSS файла вырастает до 20 килобайт и больше. Несмотря на то что он кэшируется, есть способ все же сжать сам файл. Этот пост практически перевод статьи ["The Definitive Post on Gzipping your CSS"](http://www.fiftyfoureleven.com/sandbox/weblog/2004/jun/the-definitive-css-gzip-method/) написанной [Mike Papageorge](http://www.fiftyfoureleven.com/). Здесь я опишу методы сжатия CSS файла на 70-80% с помощью PHP. Вообще говоря это можно сделать и без PHP, лишь используя модули апача: **mod\_gzip** или **mod\_deflate**. То как это можно сделать описано [тут](http://www.sitepoint.com/article/web-output-mod_gzip-apache). Если же доступа к конфигурации у вас нет (как часто бывает на хостингах), то можно воспользоваться одним из нижеследующих методов.

### Собственно сжатие

Для сжатия понадобится вот такой кусочек кода

<?php 
ob\_start ("ob\_gzhandler");
header("Content-type: text/css; charset=UTF-8");
header("Cache-Control: must-revalidate");
$offset = 60 \* 60 ;
$ExpStr = "Expires: " . 
gmdate("D, d M Y H:i:s",
time() + $offset) . " GMT";
header($ExpStr);
?>

Этот код делает следующее:

1. Использует PHPшный [ob\_gzhandler](http://es.php.net/ob_gzhandler "ob_gzhandler") для посылки сжатых данных. Эта функция сначала проверит может ли броузер принимать контент типа 'gzip,deflate' encoding;при отрицательном ответе посылает _несжатые_ данные.
2. Посылает header с content type и кодировкой файла - здесь это text/css и UTF-8.

4. Далее проверяет надо ли уже обновлять кэш для этого файла
5. Посылает информацию о том, сколько хранить файл в кэше до следующей загрузки.

### Метод первый

Первый метод заключается в переименовании вашего CSS файла в `.php`. При этом прикрепление к страничке будет выглядеть так:

  @import url(mycss.php);

Ну и в начало файла нужно добавить кусочек кода указанный выше.

### Метод второй

Второй метод чуть более универсальный. Тут не надо будет ничего менять в CSS файлах. Однако он требует правки .htaccess файла. Во-первых нужно сохранить код указанный выше, например в файл "gzip-css.php". А затем добавить в .htaccess файл следующие строки:

AddHandler application/x-httpd-php .css
php\_value auto\_prepend\_file gzip-css.php
php\_flag zlib.output\_compression On

### Пример

Я применил первый метод на зеркале ukr.net по адоесу [http://alegol.ukr.net/](http://alegol.ukr.net/). Результат себя полностью оправдал. Поскольку доступа к логам у меня нет, то я воспользовался сервисом websiteoptimisation. Результаты можно увидеть по адресам: [alegol](http://www.websiteoptimization.com/services/analyze/wso.php?url=http://alegol.ukr.net/), [ukr.net](http://www.websiteoptimization.com/services/analyze/wso.php?url=http://www.ukr.net/) В результате размер CSS файла упал с 18Кб до 4.5Кб. Жаль нельзя логи посмотреть и узнать как оно на самом деле работает при массовых нагрузках.

### Заключение

100% очень полезная штука особенно когда нет контроля над веб-сервером.

Однако есть несколько недочетов. Ходят слухи что есть какой то глюк в одной из версий ИЕ6, якобы он посылает инфу что может читать gzip, но на самом деле не раскодирует контент такого типа. Если кто то заметит подобный глюк или что то слышал об этих случаях просьба откликнуться в комменты.

Надо только еще перепроверить как оно нагружает сервер, ну а малым и средним сайтам 100% мастду.

Мну удалось найти такую инфу.

> Unfortunately, IE6 (and perhaps earlier versions?) appears to have a bug with gzip over SSL where the **first 2048 characters are not included** in the HTML rendering of the page when refresh is pressed. It only seems to happen on longish pages, and not when the page is first loaded. In fact, sometimes it doesn't happen at all. The only current solution is to put a 2048 character comment at the start of your longish pages of all spaces (which compresses pretty well, fortunately).

Однако тут имелись ввиду ХТМЛ файлы и апачевское сжатие, поэтому не знаю имеет ли это отношение к нашему случаю.
