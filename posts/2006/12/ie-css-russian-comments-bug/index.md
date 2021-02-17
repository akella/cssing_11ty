---
title: "CSS, UTF и Интернет эксплорер"
date: "2006-12-23"
humanDate: "23 Dec, 2006"
permalink: "2006/12/23/ie-css-russian-comments-bug/"
tags: 
  - "xhtmlcss"
  - "useful"
comments: 
  -  author: "dumkoeb"
     id: "6818"
     url: "http://dumkoeb.vox.com"
     date: "2006-12-23 21:30:38"
     humandate: "23 Dec, 2006"
     content: | 
       Спасибо. Я уже давно знаю этот глюк и научился его обходить. Но написать об этом как-то не додумался.

     email: "dumkoeb@gmail.com"

  -  author: "Давид Мзареулян"
     id: "6819"
     url: ""
     date: "2006-12-23 21:36:31"
     humandate: "23 Dec, 2006"
     content: | 
       А если выдавать CSS с контент-тайпом "text/css; charset=utf-8"?

     email: "david@hiero.ru"

  -  author: "Давид Мзареулян"
     id: "6820"
     url: ""
     date: "2006-12-23 21:37:03"
     humandate: "23 Dec, 2006"
     content: | 
       Т.е. windows-1251, конечно.

     email: "david@hiero.ru"

  -  author: "akella"
     id: "6821"
     url: "http://cssing.org.ua"
     date: "2006-12-23 21:39:22"
     humandate: "23 Dec, 2006"
     content: | 
       Думаю тогда все будет ок, тут как раз в том и проблема что ИЕ читает CSS в той же кодировке что и HTML страницу. При насильном указании думаю все сработает.
       
       А как вы предлагаете ее указывать? Просто ПХПшным header?

     email: "akella.a@gmail.com"

  -  author: "Макс Лапшин"
     id: "6822"
     url: "http://maxidoors.ru"
     date: "2006-12-23 22:02:24"
     humandate: "23 Dec, 2006"
     content: | 
       Почему бы не писать все в UTF8?

     email: "max@maxidoors.ru"

  -  author: "akella"
     id: "6823"
     url: "http://cssing.org.ua"
     date: "2006-12-23 22:08:27"
     humandate: "23 Dec, 2006"
     content: | 
       Тоже выход из положения, в обратную сторону проблем не возникает, но в ответ могу задать вопрос: А почему бы не windows-1251? :) Неочевидный выбор в данном случае.
       
       Одним словом я не фанат UTF.

     email: "akella.a@gmail.com"

  -  author: "Давид Мзареулян"
     id: "6824"
     url: ""
     date: "2006-12-23 22:09:07"
     humandate: "23 Dec, 2006"
     content: | 
       Настройкой веб-сервера, например.
       
       Ещё вариант:
       &lt;link rel=”stylesheet” type=”text/css” charset=”windows-1251&#8243; media=”screen,projection” href=”css/base1.css” /&gt;

     email: "david@hiero.ru"

  -  author: "alex946"
     id: "6827"
     url: ""
     date: "2006-12-23 22:49:12"
     humandate: "23 Dec, 2006"
     content: | 
       Занятно. Уже лет пять пользуюсь только UTF и ни разу не напоролся на этот баг, хотя других засад хватало. Cпасибо, будем иметь в виду. Принудительная отправка header с нужной кодировкой вроде бы помогает (ие6).

     email: "alex946@zokov.net"

  -  author: "akella"
     id: "6826"
     url: "http://cssing.org.ua"
     date: "2006-12-23 22:22:06"
     humandate: "23 Dec, 2006"
     content: | 
       В ИЕ эта строчка не помогает... думаю разве что насильно посылать header с кодировкой. Но проще уже без русских комментариев... или сам файл перегнать...
       
       Из HTML в комментах доступен только набор безопасных инлайн тагов. Жирнотсь курсив и в таком духе..

     email: "akella.a@gmail.com"

  -  author: "Zigzag"
     id: "6828"
     url: "http://lovata.com"
     date: "2006-12-23 23:21:35"
     humandate: "23 Dec, 2006"
     content: | 
       вот блин, опередил ты меня? Akella =)
       да, немало часов я потратил на поиск ответа... а помогли форумы в итоге, единственное, хорошо, что ты ответил причину бага - "съедание закрытия комментария"

     email: "zigzag85@mail.ru"

  -  author: "Mkdir"
     id: "6835"
     url: "http://exception.org.ua"
     date: "2006-12-24 03:17:32"
     humandate: "24 Dec, 2006"
     content: | 
       Я уже забыл что такое комментарии на русском ;-)

     email: "ivan.pirog@gmail.com"

  -  author: "A.I."
     id: "6841"
     url: ""
     date: "2006-12-24 07:32:33"
     humandate: "24 Dec, 2006"
     content: | 
       Кстати, наверное, из-за проблемы с кодировка не съедается */, ф просто текстовик оказывается битым (русские буквы в win1251 - это запрещенные последовательности в UTF-8).

     email: "andsit@yandex.ru"

  -  author: "akella"
     id: "6845"
     url: "http://cssing.org.ua"
     date: "2006-12-24 10:51:53"
     humandate: "24 Dec, 2006"
     content: | 
       2 A.I.: да но сути это не меняет, все что будет перед русским комментарием сработает в ИЕ, все что после - нет.
       И если где то после русского комментария в файле, у тебя будет еще один комментарий(уже без русских букв) - то не сработают только правила между двумя этими комментариями. Из этого я как раз и сделал выводы о том, что комментарий остается открытым для ИЕ. Все указывает на это.
       Вот пример, после второго комментария я указал красный фон для body - http://cssing.org.ua/examples/iecssutf/indexUTF2com.html, и вот такой там CSS:
       http://cssing.org.ua/examples/iecssutf/css/base2comments.css
       
       2Mkdir: поверь, в том файле у меня было около 20 комментариев, и только в одном из них я употребил русскую букву...:) Я был в миллиметре от благополучного исхода..

     email: "akella.a@gmail.com"

  -  author: "Mkdir"
     id: "6869"
     url: "http://exception.org.ua"
     date: "2006-12-25 15:15:36"
     humandate: "25 Dec, 2006"
     content: | 
       2Akella: Прикольно =)
       Кстати, можно ведь и опечататься, например набрав вместо английской 'c' русскую 'c', которые находятся на одной и той же клавише в обоих раскладках...
       Ну что тут сказать. Internet Explorer, индусы...

     email: "ivan.pirog@gmail.com"

  -  author: "yoppt"
     id: "6873"
     url: "http://yoppt.spb.ru"
     date: "2006-12-25 23:35:26"
     humandate: "25 Dec, 2006"
     content: | 
       вы бы еще по-монгольски комментарии написали.

     email: "mail@yoppt.spb.ru"

  -  author: "akella"
     id: "6874"
     url: "http://cssing.org.ua"
     date: "2006-12-25 23:40:03"
     humandate: "25 Dec, 2006"
     content: | 
       То есть родной язык в кодировке используемой самой популярной ОС, вы сравнили с монгольским? Замечательное и логичное сравнение. Спасибо!

     email: "akella.a@gmail.com"

  -  author: "YoYurec"
     id: "6882"
     url: "http://yoyurec.in.ua/"
     date: "2006-12-26 12:35:08"
     humandate: "26 Dec, 2006"
     content: | 
       спасибо, возьму на заметку!

     email: "yoyurec@gmail.com"

  -  author: "EL"
     id: "6896"
     url: ""
     date: "2006-12-27 06:23:27"
     humandate: "27 Dec, 2006"
     content: | 
       напоролся на этот глюк пару лет назад еще

     email: "i.butylsky@office.ngs.ru"

  -  author: "Dimox"
     id: "7054"
     url: "http://dimox.biz"
     date: "2007-01-02 16:43:46"
     humandate: "02 Jan, 2007"
     content: | 
       Премного благодарен! Действительно, не зная об этом баге можно потратить уйму времени, пытаясь найти причину.
       
       Хотя комменты и пишу латиницей, про такой глюк не знал. Теперь буду иметь в виду.

     email: "suprabiz@mail.ru"

  -  author: "системы видеонаблюдения"
     id: "7202"
     url: "http://kbbezopasnosti.ru/video/"
     date: "2007-01-09 11:14:59"
     humandate: "09 Jan, 2007"
     content: | 
       можно в .htaccess прописать кодировку...

     email: "sx189@yandex.ru"

  -  author: "SvT"
     id: "8063"
     url: "http://svt.name"
     date: "2007-02-07 19:03:39"
     humandate: "07 Feb, 2007"
     content: | 
       спасибо, интересно)

     email: "spaming@gmail.com"

  -  author: "Yuriy"
     id: "8218"
     url: "http://blog.sribna.com"
     date: "2007-02-12 19:20:05"
     humandate: "12 Feb, 2007"
     content: | 
       Логично при указании кодировки страницы utf-8 и .css файл сохранить в этой же кодировке.

     email: "y.drozdov@gmail.com"

  -  author: "akella"
     id: "8219"
     url: "http://cssing.org.ua"
     date: "2007-02-12 19:22:56"
     humandate: "12 Feb, 2007"
     content: | 
       Это точно, только вот делаются эти вещи(кодировка страниц и CSS файлы) как правило разными людьми. И подобная практика не так очевидна, хотя и логична.

     email: "akella.a@gmail.com"

  -  author: "alex"
     id: "8893"
     url: "http://www.spb-events.ru"
     date: "2007-02-27 21:46:09"
     humandate: "27 Feb, 2007"
     content: | 
       Подскажите где лажа при отображении в IE на сайте http://www.magshar.ru/ в опере всё окей естественно

     email: "info@spb-events.ru"

  -  author: "Заметки юного фрилансера! &raquo; Div верстка и InternetExplorer 6&nbsp;&mdash; гримучая смесь!"
     id: "14669"
     url: "http://freeman.pp.ua/2009/07/26/div-verstka-i-internetexplorer-6-grimuchaya-smes/"
     date: "2009-07-26 19:11:23"
     humandate: "26 Jul, 2009"
     content: | 
       [...] А узнал я это с http://cssing.org.ua/2006/12/23/ie-css-russian-comments-bug/ [...]

     email: ""

  -  author: "Daemon"
     id: "10901"
     url: "http://ivg.dp.ua/"
     date: "2007-04-13 15:55:29"
     humandate: "13 Apr, 2007"
     content: | 
       Или оставлять пробел перед закрытием комментария.

     email: "ilya.daemon@gmail.com"

  -  author: "html верстка"
     id: "10908"
     url: "http://www.fasthtml.ru"
     date: "2007-04-16 21:09:38"
     humandate: "16 Apr, 2007"
     content: | 
       есть другое решение проблемы,
       добавить в начало css файла правило:
       
        @charset "windows-1251";
       
       Пример: 
       http://www.fasthtml.ru/examples/ie/indexUTF.html
       
       Спецификация: 
       http://www.w3.org/TR/REC-CSS2/syndata.html#q23

     email: "anasyrov@fasthtml.ru"

  -  author: "John"
     id: "11093"
     url: ""
     date: "2007-07-26 14:07:10"
     humandate: "26 Jul, 2007"
     content: | 
       А что будет в такой же ситуации но с файлом скриптов? Т.е. сайт в кодировке UTF и к нему цепляется js файл, у которого внутри сообщения и/или комментарии по-русски в Win-1251.

     email: "john@smith.com"

  -  author: "Vladimir"
     id: "11194"
     url: "http://www.coolthemes.ru"
     date: "2007-10-08 08:40:00"
     humandate: "08 Oct, 2007"
     content: | 
       Пытаюсь собрать сайт.
       Под FireFox все смотрится гуд, а вот под ИЕ над верхней шапкой
       появляется пустое место и внизу пропадает выравнивание, хотя при
       переходе на любой внутренний раздел все встает на места.
       
       http://www.cmagister.info/
       
       Может быть вы сталкивались с таким ?
       Заранее спасибо.

     email: "vladimir@tatarovich.ru"

  -  author: "akella"
     id: "11195"
     url: "http://cssing.org.ua"
     date: "2007-10-09 01:42:24"
     humandate: "09 Oct, 2007"
     content: | 
       Сделайте код валидным прежде чем думать об ошибках ИЕ.
       
       Я этот глюк наблюдаю и в Сафари, скорее всего лишний раз закрыт или не закрыт ДИВ или другой элемент.

     email: "akella.a@gmail.com"

  -  author: "akella"
     id: "11296"
     url: "http://cssing.org.ua"
     date: "2007-11-10 14:05:58"
     humandate: "10 Nov, 2007"
     content: | 
       Посмотрите в какой кодировке отсылает вам сервер страничку

     email: "akella.a@gmail.com"

  -  author: "Вадим Макишвили"
     id: "11633"
     url: "http://makishvili.ya.ru"
     date: "2008-01-09 19:06:15"
     humandate: "09 Jan, 2008"
     content: | 
       Юра, привет. 
       Есть еще одно решение в добавок к твоим двум.
       В файле с cp1251 после русского комментария добавить пустой коммент:
       /* русский коммент */ /**/
       
       Проверено на Я.Ру :)
       
       Это решение мне пришло в голову, когда я прочитал твое предположние, что съедается символ закрытия. После еще одного пустого коммента в той же строке - проблема исчезает.

     email: "makishvili@yandex.ru"

  -  author: "Чингис"
     id: "12398"
     url: "http://pula.com.ua"
     date: "2008-05-08 09:02:43"
     humandate: "08 May, 2008"
     content: | 
       даааа
        все утро искал проблему - теперь нашел внятным языком и где )
       
        спасибо друг

     email: "chingis@pula.com.ua"

  -  author: "Сергей"
     id: "14479"
     url: "http://www.moreraboty.com"
     date: "2009-06-09 15:33:10"
     humandate: "09 Jun, 2009"
     content: | 
       Спасибо просто огромное!!!
       А то стили упорно не хотели работать в 6 ослике именно по этой причине.

     email: "vip@dsip.net"

  -  author: "Илья"
     id: "12968"
     url: "http://!"
     date: "2008-07-27 09:20:20"
     humandate: "27 Jul, 2008"
     content: | 
       Спасибо!!!!!

     email: "ava@ukr.net"

  -  author: "Олег"
     id: "13169"
     url: "http://www.htmlverstka.ru"
     date: "2008-08-30 23:17:09"
     humandate: "30 Aug, 2008"
     content: | 
       Можно сделать проще, не комментировать css :)), а вообще чем проще тем лучше, назвать класс в тему и не надо комментировать, пример htmlverstka.ru

     email: "a11_1@mail.ru"

  -  author: "Vitaly Harisov"
     id: "13319"
     url: "http://vitaly.harisov.name"
     date: "2008-09-30 22:36:56"
     humandate: "30 Sep, 2008"
     content: | 
       <blockquote>Можно сделать проще, не комментировать css :)), а вообще чем проще тем лучше, назвать класс в тему и не надо комментировать, пример htmlverstka.ru</blockquote>
       
       Не смешно.

     email: "vitaly@harisov.name"

layout: "layouts/post.njk"
excerpt: "Недавно я и некоторые из моих знакомых напоролись на интересный неочевидный глюк связанный с употреблением русских комментариев в CSS. Суть глюка и пример ниже. Сразу резюме: <strong>лучше не используйте комментарии с кириллицей в CSS</strong>.
"
---

Недавно я и некоторые из моих знакомых напоролись на интересный неочевидный глюк связанный с употреблением русских комментариев в CSS. Суть глюка и пример ниже. Сразу резюме: <strong>лучше не используйте комментарии с кириллицей в CSS</strong>.
<!--more-->
<h3>Ответа в инете не нашел</h3>
Наверняка многие на него  напарывались - но внятного ответа от гугла мне получить не удалось - потому я решил для экономии времени читателей озвучить этот гадкий и противный глюк. По незнанию такого глюка отладка может быть длительной. Глюк проявляется только в версиях интернет эксплорера 5.0-6.0
<h3>Типичная ситуация для бага</h3>
Вы верстаете сайт. Кодировка ваших CSS файлов по умолчанию выставлена windows-1251. После чего верстка попадает в реализацию, где она прикручивается к движку(в движке HTML отдается как UTF-8). Однако оказывается, что в ИЕ6 и ниже, сайт сильно расползается и часть CSS не работает. Причина - русские комментарии в CSS. 
<h3>Пример</h3>
Для примера я создал CSS файл с русскими комментариями в кодировке windows-1251:
<ol class="code">
<li>/*Русский комментарий*/</li>
<li>#content{</li>
<li>color:#fff;</li>
<li>background:#000;</li>
<li>}</li>
</ol>
И две HTML странички(<a  href="http://cssing.org.ua/examples/iecssutf/">страничка в windows-1251</a> и <a href="http://cssing.org.ua/examples/iecssutf/indexUTF.html">страничка в UTF-8</a>), отличающиеся лишь метатагами
<ol class="code">
<li>&lt;meta http-equiv=&quot;content-type&quot; content=&quot;text/html; charset=utf-8&quot;&gt;</li>
</ol>
И
<ol class="code">
<li>&lt;meta http-equiv=&quot;Content-Type&quot; content=&quot;text/html; charset=windows-1251&quot; /&gt;</li>
</ol>
Обе странички ссылаются на один и тот же <a href="http://cssing.org.ua/examples/iecssutf/css/base.css">CSS файл</a>. В результате в ИЕ6 и ниже, CSS на страничке с кодировкой UTF не срабатывает. Все из-за русских комментариев.
<h3>Решение</h3>
Есть несколько путей:
<ul>
<li>Удалить русские комментарии из CSS</li>
<li>Поменять кодировку CSS файла на UTF-8</li>
</ul>
Но лучше никогда не использовать кириллицу для комментирования CSS файлов. Мало ли к чему там будут прикручивать потом вашу верстку... а кодировку CSS файлов догадаются поменять в последнюю очередь.

Суть бага в том, что при наличии русского комментария(UTF кодировка страницы переносится и на CSS), IE сьедает символ закрытия комментария, в результате весь CSS после русских букв оказывается так же закомментированным. В IE7 этот "баг" не проявляется. Примеры смотреть в  IE 6  и ниже.
<h3>Ссылки</h3>
<ul>
<li><a href="http://cssing.org.ua/examples/iecssutf/">Страничка и CSS файл в кодировке windows-1251</a></li>
<li><a href="http://cssing.org.ua/examples/iecssutf/indexUTF.html">Страничка в кодировке UTF-8, CSS файл в кодировке windows-1251</a></li>
<li><a href="http://cssing.org.ua/examples/iecssutf/UTFnoRussianText.html">Страничка в кодировке UTF-8, CSS файл в кодировке windows-1251 без русских комментариев</a></li>
</ul>
Надеюсь,  по крайней мере те кто это прочитают, не потратят теперь пару часов своей жизни на поиск такого бага. Будьте внимательны! Буду рад, если Вы поделитесь своим опытом по этому поводу.
