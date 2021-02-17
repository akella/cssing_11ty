---
title: "Как сжимать CSS"
date: "2005-04-07"
humanDate: "07 Apr, 2005"
permalink: "2005/04/07/gzipping-your-css/"
tags: 
  - "perevod"
  - "useful"
comments: 
  -  author: "DiGiTAL"
     id: "1652"
     url: "http://pomaranch.info"
     date: "2005-04-30 02:49:11"
     humandate: "30 Apr, 2005"
     content: | 
       нашел и разобрался... просто не было необходимости пользоваться, так что предыдущие комменты прошу удалить, как флуд ;)

     email: "digital@pomaranch.info"

  -  author: "DiGiTAL"
     id: "1653"
     url: "http://pomaranch.info"
     date: "2005-04-30 02:51:48"
     humandate: "30 Apr, 2005"
     content: | 
       по поводу второго метода:
       а что делать, если хостер отключил установки пхп для хаткасов?
       идея просто понравилась... а реализовать - никак... и надо не для цсс совсем

     email: "digital@pomaranch.info"

  -  author: "akella"
     id: "1663"
     url: "http://cssing.iatp.org.ua"
     date: "2005-04-30 18:29:24"
     humandate: "30 Apr, 2005"
     content: | 
       тогда как по мне проще заставить его юзать mod_gzip или deflate. Или связаться с хостером, тока надо на хорошее настроение попасть :). 
       Ниче более дельного не знаю :(

     email: "akella.a@gmail.com"

  -  author: "ganges"
     id: "1329"
     url: ""
     date: "2005-04-09 10:42:07"
     humandate: "09 Apr, 2005"
     content: | 
       Нормально работает, действительно можно сжимать. Вот только быстро привыкаешь :) и перестаешь париться насчет размера файлов, а это имеет, как ты понимаешь, последствия. Поэтому, имхо, надо просто стараться писать короткий CSS, что в случае с Укрнет, конечно, врядли возможно. Я стараюсь писать суммарный CSS не более 12 килобайт, пока получается :)

     email: "andrey.stefanenko@gmail.com"

  -  author: "mourner"
     id: "1332"
     url: ""
     date: "2005-04-09 20:22:54"
     humandate: "09 Apr, 2005"
     content: | 
       Кстати, только что заметил, что у тебя линк на css validator в футере поломан. :-)

     email: "equi@nospam.com"

  -  author: "akella"
     id: "1348"
     url: "http://cssing.iatp.org.ua"
     date: "2005-04-10 13:58:12"
     humandate: "10 Apr, 2005"
     content: | 
       знаю знаю
       Спсб - боюсь что не пройду валидацию ;) 
       скоро исправлю...

     email: "akella.a@gmail.com"

  -  author: "tobto_"
     id: "2894"
     url: "http://tobto.com.ua"
     date: "2006-03-14 16:18:26"
     humandate: "14 Mar, 2006"
     content: | 
       а засунуть css в кеш с помощью javascript?

     email: "info@eurosong2006.net"

  -  author: "W@D"
     id: "2897"
     url: "http://wadowad.narod.ru"
     date: "2006-03-18 01:41:26"
     humandate: "18 Mar, 2006"
     content: | 
       А разве CSS не в кэше?! (вопрос риторический)

     email: "wadowad@rambler.ru"

  -  author: "Aleko"
     id: "14841"
     url: "http://studioad.ru"
     date: "2009-10-16 17:37:37"
     humandate: "16 Oct, 2009"
     content: | 
       Можно ещё так оптимизировать: http://studioad.ru/blog/szhimaem_css_algoritmom_base62/2009-10-16-97

     email: "admin@studioad.ru"

  -  author: "Тормоз"
     id: "11152"
     url: "http://BrokenBrake.biz"
     date: "2007-08-30 14:22:42"
     humandate: "30 Aug, 2007"
     content: | 
       Попробовал у себя сделать - CSS вообще грузиться перестали. Жаль.

     email: "BrokenBrake@gmail.com"

  -  author: "Тормоз"
     id: "11151"
     url: "http://BrokenBrake.biz"
     date: "2007-08-30 14:04:42"
     humandate: "30 Aug, 2007"
     content: | 
       Привет! Твой блог знаю уже не первый год, но на этот раз пришел с поисковика, и нашел именно то, что искал :) Спасибо!

     email: "BrokenBrake@gmail.com"

  -  author: "gugglegum"
     id: "11162"
     url: "http://web-notes.ru"
     date: "2007-09-12 08:35:53"
     humandate: "12 Sep, 2007"
     content: | 
       Во-первых, выдавать CSS при помощи PHP -- это дико с точки зрения нагрузки на веб-сервер.
       
       Во-вторых, Ваш первый метод увеличивает время загрузки на 1 GET-запрос. И на самом деле это не нужно, Вы можете в самом HTML прописать ссылку не на CSS, а на PHP-файл. Так будет проще, быстрее и естественнее.
       
       В-третьих, доступ к серверу на нормальных хостингах все же есть. И если у нас есть доступ к .htaccess, используемому во втором методе, то наверняка мы там же можем заюзать и mod_deflate.
       
       В-четвертых, Ваш метод хоть и реализует сжатие CSS, но при этом почти сводит на нет кэширование. Вы используете только Expiration Model кэширования, а по истечению срока вынуждаете браузер загружать CSS заново, даже если он не изменился.
       
       Я предлагаю свой вариант. Я просто модифицировал один свой старый исходник, сейчас у меня есть более совершенный способ, но он слишком большой для постинга сюда. Мой вариант использует сразу обе модели кэширования: Expiration и Validation. В течение 24 часов CSS будет лежать в кэше и браузер даже не будет обращаться к серверу, а по истечении 24 часов браузер пошлет условный запрос, который вернет CSS только, если он с тех пор изменился, либо HTTP/1.1 304 Not Modified, если нет.
       
       Мой вариант использует mod_rewrite. Лично я использую исключительно его при написании веб-приложений, поэтому его наличие на сервере для меня -- как стандарт де-факто. Я просто ставлю в технические требования к веб-серверу наличие этого модуля. Итак, в .htaccess пишем:
       
       RewriteEngine on
       RewriteCond %{REQUEST_FILENAME} -f
       RewriteRule \.css$ cssfilter.php
       
       а в cssfilter.php:
       
       <code>
       
       
        */
       
       // assume that REQUEST_URI contains short URI from document root
       $file = $_SERVER['DOCUMENT_ROOT'].$_SERVER['REQUEST_URI'];
       
       // we don't have to warn about file existing because rewrite rule guarantees that.
       if (($content = file_get_contents($file)) !== false)
       {
        // handle HTTP request header If-Modified-Since (simulating static content)
        $lastmod = filemtime($file);
        if (isset($_SERVER['HTTP_IF_MODIFIED_SINCE']))
        {
        $modsince = strtotime($_SERVER['HTTP_IF_MODIFIED_SINCE']);
        if ($modsince != -1 &amp;&amp; $modsince == $lastmod)
        {
        header($_SERVER['SERVER_PROTOCOL'].' 304 Not Modified');
        header('Content-Type: text/css');
        exit();
        }
        }
       
        $maxAge = 3600 * 24;
        header('Expires: '.gmdate("D, d M Y H:i:s", time() + $maxAge) . " GMT");
        header('Cache-Control: public; max-age='.$maxAge);
        header('Last-Modified: '.gmdate("D, d M Y H:i:s", $lastmod) . " GMT");
        header('Content-Type: text/css');
       
        // output CSS file
        ob_start('gz_handler');
        echo $content;
        ob_end_flush();
       }
       else // we should never reach this condition (only if some hardware error)
        echo "Read file error";
       
       ?&gt;
       
       </code>

     email: "gugglegum@gmail.com"

  -  author: "gugglegum"
     id: "11163"
     url: "http://web-notes.ru"
     date: "2007-09-12 08:41:06"
     humandate: "12 Sep, 2007"
     content: | 
       Мда... Форматирование кода сломалось, и комментарий почему-то удалился, остался только закрывающий комментарий в начале...

     email: "gugglegum@gmail.com"

  -  author: "DfK"
     id: "11240"
     url: ""
     date: "2007-10-26 16:06:03"
     humandate: "26 Oct, 2007"
     content: | 
       мм, не знаю, у меня текст сжимается не меньше чем в 10 раз;)

     email: "senko@list.ru"

  -  author: "Taras"
     id: "11501"
     url: ""
     date: "2007-12-19 22:39:01"
     humandate: "19 Dec, 2007"
     content: | 
       из 11 поста не работает в FireFox

     email: "nEH3iH@ya.ru"

  -  author: "ScorpAL"
     id: "11870"
     url: ""
     date: "2008-02-27 15:20:51"
     humandate: "27 Feb, 2008"
     content: | 
       http://dev.wp-plugins.org/wiki/css-compress
       
       CSS Compress - плагин для WordPress для сжатия CSS в GZip

     email: "scorpal@gmail.com"

  -  author: "BOLK"
     id: "13645"
     url: "http://bolknote.ru"
     date: "2008-11-20 14:50:37"
     humandate: "20 Nov, 2008"
     content: | 
       Тут ошибка:
       header("Content-type: text/css; charset: UTF-8");
       
       Должно быть:
       header("Content-type: text/css; charset=UTF-8");

     email: "imbolk@gmail.com"

  -  author: "akella"
     id: "13647"
     url: "http://cssing.org.ua"
     date: "2008-11-20 20:45:25"
     humandate: "20 Nov, 2008"
     content: | 
       Спасибо! Поправил!

     email: "akella.a@gmail.com"

layout: "layouts/post.njk"
excerpt: "Иногда на больших сайтах размер CSS файла вырастает до 20 килобайт и больше. Несмотря на то что он кэшируется, есть способ все же сжать сам файл. Этот пост практически перевод статьи <a href=\"http://www.fiftyfoureleven.com/sandbox/weblog/2004/jun/the-definitive-css-gzip-method/\">\"The Definitive Post on Gzipping your CSS\"</a> написанной <a href=\"http://www.fiftyfoureleven.com/\">Mike Papageorge</a>. "
---

Иногда на больших сайтах размер CSS файла вырастает до 20 килобайт и больше. Несмотря на то что он кэшируется, есть способ все же сжать сам файл. Этот пост практически перевод статьи <a href="http://www.fiftyfoureleven.com/sandbox/weblog/2004/jun/the-definitive-css-gzip-method/">"The Definitive Post on Gzipping your CSS"</a> написанной <a href="http://www.fiftyfoureleven.com/">Mike Papageorge</a>. <!--more-->
Здесь я опишу методы сжатия CSS файла на 70-80% с помощью PHP. Вообще говоря это можно сделать и без PHP, лишь используя модули апача: <strong>mod_gzip</strong> или <strong>mod_deflate</strong>. То как это можно сделать описано<a href="http://www.sitepoint.com/article/web-output-mod_gzip-apache"> тут</a>. Если же доступа к конфигурации у вас нет (как часто бывает на хостингах), то можно воспользоваться одним из нижеследующих методов.
<h3>Собственно сжатие</h3>
Для сжатия понадобится вот такой кусочек кода
<pre>
&lt;?php 
ob_start (&quot;ob_gzhandler&quot;);
header(&quot;Content-type: text/css; charset=UTF-8&quot;);
header(&quot;Cache-Control: must-revalidate&quot;);
$offset = 60 * 60 ;
$ExpStr = &quot;Expires: &quot; . 
gmdate(&quot;D, d M Y H:i:s&quot;,
time() + $offset) . &quot; GMT&quot;;
header($ExpStr);
?&gt;
</pre>
Этот код делает следующее:
<ol><li>Использует  PHPшный <a href="http://es.php.net/ob_gzhandler" title="ob_gzhandler">ob_gzhandler</a> для посылки сжатых данных. Эта функция сначала проверит может ли броузер принимать контент типа  &#39;gzip,deflate&#39; encoding;при отрицательном ответе посылает <em>несжатые</em> данные.
</li>
<li>Посылает  header с content type и кодировкой файла - здесь это text/css и UTF-8.</li>

<li>Далее проверяет надо ли уже обновлять кэш для этого файла</li>
<li>Посылает информацию о том, сколько хранить файл в кэше до следующей загрузки.</li> </ol>
<h3>Метод первый</h3>
Первый метод заключается в переименовании вашего CSS файла в <code>.php</code>. При этом прикрепление к страничке будет выглядеть так:
<pre>
  @import url(mycss.php);
</pre>
Ну и в начало файла нужно добавить кусочек кода указанный выше.
<h3>Метод второй</h3>
Второй метод чуть более универсальный. Тут не надо будет ничего менять в CSS файлах. Однако он требует правки .htaccess файла.
Во-первых нужно сохранить код указанный выше, например в файл "gzip-css.php".
А затем добавить в .htaccess файл следующие строки:
<pre>
AddHandler application/x-httpd-php .css
php_value auto_prepend_file gzip-css.php
php_flag zlib.output_compression On
</pre>
<h3>Пример</h3>
Я применил первый метод на зеркале ukr.net по адоесу<a href="http://alegol.ukr.net/"> http://alegol.ukr.net/</a>. Результат себя полностью оправдал.
Поскольку доступа к логам у меня нет, то я воспользовался сервисом websiteoptimisation.
Результаты можно увидеть по адресам:
<a href="http://www.websiteoptimization.com/services/analyze/wso.php?url=http://alegol.ukr.net/">alegol</a>,
<a href="http://www.websiteoptimization.com/services/analyze/wso.php?url=http://www.ukr.net/">ukr.net</a>
В результате размер CSS файла упал с 18Кб до 4.5Кб. Жаль нельзя логи посмотреть и узнать как оно на самом деле работает при массовых нагрузках.
<h3>Заключение</h3>
100% очень полезная штука особенно когда нет контроля над веб-сервером.

Однако есть несколько недочетов. Ходят слухи что есть какой то глюк в одной из версий ИЕ6, якобы он посылает инфу что может читать gzip, но на самом деле не раскодирует контент такого типа. Если кто то заметит подобный глюк или что то слышал об этих случаях просьба откликнуться в комменты. 

Надо только еще перепроверить как оно нагружает сервер, ну а малым и средним сайтам 100% мастду.

Мну удалось найти такую инфу. 
<blockquote>Unfortunately, IE6 (and perhaps earlier versions?) appears to have a bug with gzip over SSL where the <strong>first 2048 characters are not included</strong> in the HTML rendering of the page when refresh is pressed. It only seems to happen on longish pages, and not when the page is first loaded. In fact, sometimes it doesn't happen at all. The only current solution is to put a 2048
character comment at the start of your longish pages of all spaces (which compresses pretty well, fortunately).</blockquote>

Однако тут имелись ввиду ХТМЛ файлы и апачевское сжатие, поэтому не знаю имеет ли это отношение к нашему случаю.
