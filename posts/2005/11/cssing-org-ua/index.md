---
title: "cssing.org.ua"
date: "2005-11-10"
humanDate: "10 Nov, 2005"
permalink: "2005/11/10/cssing-org-ua/"
tags: 
  - "common"
comments: 
  -  author: "Vladson"
     id: "2557"
     url: "http://dkflbk.nm.ru/"
     date: "2005-11-10 20:22:35"
     humandate: "10 Nov, 2005"
     content: | 
       Шустрый хостинг, поздравляю, а то тормоза были немерянные (я тоже из неукраинцев)

     email: "dkflbk@nm.ru"

  -  author: "kost"
     id: "2555"
     url: "http://reg.kost.ru"
     date: "2005-11-10 12:27:43"
     humandate: "10 Nov, 2005"
     content: | 
       &gt;Кроме того тот хостинг грешил медлительностью для неукраинцев - узкий канал.
       
       Да, сейчас гораздо лучше.

     email: "kost@kost.ru"

  -  author: "Александр"
     id: "2556"
     url: ""
     date: "2005-11-10 13:30:11"
     humandate: "10 Nov, 2005"
     content: | 
       С новосельем!
       Хостинг намного лучше, сильно шустрее! -)

     email: "vaklhov@km.ru"

  -  author: "tobto_"
     id: "2559"
     url: "http://tobto.com.ua"
     date: "2005-11-11 23:54:08"
     humandate: "11 Nov, 2005"
     content: | 
       Привет от Тобто! 
       
       Я лично в этом году сменил хостинг на другие американские сервера :) - сервис супер - cpanel, etc. - посмотрите whois: http://www.whois.sc/eurosong2006.net - сервера UKRAINEHOSTING находятся в Чехасе. Рекомендую. Отзыв моментальный. Я без особенной рекламы. Прошел хостинг iptelecom, svitonline, hostpro.com.ua,... 
       Адрес такой: besthosting.com.ua
       
       Chiao!

     email: "info@eurosong2006.net"

  -  author: "Vladson"
     id: "2570"
     url: "http://dkflbk.nm.ru/"
     date: "2005-11-13 23:19:24"
     humandate: "13 Nov, 2005"
     content: | 
       По поводу реврайта лучше сделай редирект через HTTP-301 (PR тогда передёт от туда сюда)
       
       http://forum.searchengines.ru/showthread.php?t=29292

     email: "dkflbk@nm.ru"

  -  author: "akella"
     id: "2576"
     url: "http://cssing.org.ua"
     date: "2005-11-14 11:00:15"
     humandate: "14 Nov, 2005"
     content: | 
       Я почему использовал мод-реврайт - что бы урлы типа <strong>cssing.iatp.org.ua/feed/</strong> перенаправлялись на <strong>cssing.org.ua/feed/</strong>. Что бы старые линки все разом не перестали работать - много поссылаться успели на меня... :(
       
       А тут получается нельзя будет такой редирект? Или я неправ?

     email: "akella.a@gmail.com"

  -  author: "Vladson"
     id: "2578"
     url: "http://dkflbk.nm.ru/"
     date: "2005-11-14 12:00:44"
     humandate: "14 Nov, 2005"
     content: | 
       Такой можно но только если сделать грамотно 
       
       (реврайтом на РНР скрипт перенаправлять, а из скрипта грамотный редирект на этот сайт...)
       Типа того что
       
       RewriteEngine On
       RewriteCond ^(тря-ля-ля)$ index.php?str=$1
       
       А в скрипте
       
       
       
       Это естественно упрощенно (писал на ходу, не помню точно подробностей как там это делается, надо в шпаргалку глянуть)

     email: "dkflbk@nm.ru"

  -  author: "Vladson"
     id: "2579"
     url: "http://dkflbk.nm.ru/"
     date: "2005-11-14 12:02:41"
     humandate: "14 Nov, 2005"
     content: | 
       А в скрипте (в прошлый раз вырезал, попробую обойти защиту)
       
       (?php
       header('тра-ля-ля: три рубля' . $_GET['str'] );
       ?)

     email: "dkflbk@nm.ru"

  -  author: "akella"
     id: "2582"
     url: "http://cssing.org.ua"
     date: "2005-11-14 12:31:51"
     humandate: "14 Nov, 2005"
     content: | 
       Спасибо большое - путь увидел. Сегодня же попытаюсь провернуть - если еще мой старый ПР не обнулили окончательно. 
       Какой-то полубредовый тул "pagerank prediction" обещает мне ПР 8. Врунишка. :)
       
       А есть что то по поводу того что мой первый мод-реврайт не передаст ПР?
       
       Ведь в твоем варианте все тоже сводится к реврайтам?

     email: "akella.a@gmail.com"

  -  author: "Vladson"
     id: "2583"
     url: "http://dkflbk.nm.ru/"
     date: "2005-11-14 12:41:55"
     humandate: "14 Nov, 2005"
     content: | 
       PR перенаправляется редиректом 301-го HTTP заголовка, а реврайт делает перенаправление не совсем так (точнее совсем не так, а стало быть поисковики не будут видеть этого перенаправления)

     email: "dkflbk@nm.ru"

  -  author: "akella"
     id: "2584"
     url: "http://cssing.org.ua"
     date: "2005-11-14 16:54:54"
     humandate: "14 Nov, 2005"
     content: | 
       Все оказалось несколько проще, без участия ПХП
       http://www.webmasterworld.com/forum92/4785.htm
       Нужно лишь исправить строку:
       <ol class="code" style="margin:0;padding-left:0;">
       <li>...</li>
       <li>RewriteRule ^(.*)$ http://cssing.org.ua/$1 <del>[R]</del> [R=301,L]</li>
       <li>...</li>
       </ol>

     email: "akella.a@gmail.com"

  -  author: "Vladson"
     id: "2585"
     url: "http://dkflbk.nm.ru/"
     date: "2005-11-14 23:49:53"
     humandate: "14 Nov, 2005"
     content: | 
       Да пожалуй так, я просто не очень часто занимаюсь реврайтом по этому не помню как действуют ключ [R], а в шпаргалку (мануал) не заглядывал... 
       (был уверен что ты и сам достаточно квалифицирован, и я не ошибался)

     email: "dkflbk@nm.ru"

  -  author: "Poster"
     id: "2586"
     url: "http://www.dima.design.lviv.ua"
     date: "2005-11-16 12:41:27"
     humandate: "16 Nov, 2005"
     content: | 
       У меня так:
       
       RewriteEngine on
       RewriteCond %{HTTP_HOST} ^carpathians.com.ua$ [OR]
       RewriteCond %{HTTP_HOST} ^www.carpathians.com.ua$
       RewriteRule ^(.*)$ http://www.design.lviv.ua [R=301,L]

     email: "svaryk@ua.fm"

  -  author: "zaartix"
     id: "2592"
     url: "http://zaartix.ru"
     date: "2005-11-23 23:57:30"
     humandate: "23 Nov, 2005"
     content: | 
       А чем плох такой вариант:
       Redirect permanent / http://cssing.org.ua/
       
       гораздо проще и без лишних хлопот

     email: "zaartix@yandex.ru"

  -  author: "akella"
     id: "2593"
     url: "http://cssing.org.ua"
     date: "2005-11-24 12:36:24"
     humandate: "24 Nov, 2005"
     content: | 
       А разве в этом случае было бы перенаправление
       http://cssing.iatp.org.ua/2005/11/10/cssing-org-ua/
       на
       http://cssing.org.ua/2005/11/10/cssing-org-ua/
       ?
       Я хотел сохранить все старые ссылки рабочими, не только те что вели на главную...

     email: "akella.a@gmail.com"

  -  author: "Alexey"
     id: "2616"
     url: "http://zaartix.ru"
     date: "2005-11-29 10:00:19"
     humandate: "29 Nov, 2005"
     content: | 
       А Вы бы попробовали. 
       Ес-но было-бы и такое перенаправление, даже более того, если бы где-то была ссылка на картинку то она бы показалась с нового места.

     email: "zaartix@yandex.ru"

  -  author: "zaARTix"
     id: "2617"
     url: "http://zaartix.ru"
     date: "2005-11-29 10:01:10"
     humandate: "29 Nov, 2005"
     content: | 
       Сорри, предыдущий пост от меня.

     email: "zaartix@yandex.ru"

  -  author: "akella"
     id: "2621"
     url: "http://cssing.org.ua"
     date: "2005-11-29 14:53:57"
     humandate: "29 Nov, 2005"
     content: | 
       Да, спасибо большое - я из-за такой простоты и не поверил сразу :)
       Добавил в пост.

     email: "akella.a@gmail.com"

  -  author: "maximum"
     id: "2643"
     url: "http://blog.crime.su"
     date: "2005-12-07 09:56:43"
     humandate: "07 Dec, 2005"
     content: | 
       Прально, через 301 редирект делать.

     email: "iframe@list.ru"

  -  author: "пятка"
     id: "2694"
     url: "http://mouldframe.com"
     date: "2006-01-06 15:05:28"
     humandate: "06 Jan, 2006"
     content: | 
       такой вариант тоже подходит.

     email: "dead-proxor@mouldframe.com"

  -  author: "пятка"
     id: "2695"
     url: "http://mouldframe.com"
     date: "2006-01-06 15:58:30"
     humandate: "06 Jan, 2006"
     content: | 
       код не вставило

     email: "dead-proxor@mouldframe.com"

  -  author: "akella"
     id: "2696"
     url: "http://cssing.org.ua"
     date: "2006-01-06 17:00:22"
     humandate: "06 Jan, 2006"
     content: | 
       Надо было позаменять знак &gt; на &amp;gt; и в таком роде... :(

     email: "akella.a@gmail.com"

  -  author: "Иван"
     id: "15007"
     url: ""
     date: "2009-12-18 23:22:43"
     humandate: "18 Dec, 2009"
     content: | 
       besthosting.ua - кидало 21 века! толпа, как вылечить бешанного пса (Варшавский Р.В.)?

     email: "tv5@bigmir.ua"

layout: "layouts/post.njk"
excerpt: "Переехал. Хостинг стал напрягать своими проблемами. Надеюсь здесь будет намного уютнее :). Кроме того тот хостинг грешил медлительностью для неукраинцев - узкий канал. Тут вроде ровнее.
(Менять айпишник на cssing.iatp.org.ua мне \"типа\" отказали.) Для переезда использовал мод_реврайт, надеюсь это окажется кому-то полезным.  "
---

Переехал. Хостинг стал напрягать своими проблемами. Надеюсь здесь будет намного уютнее :). Кроме того тот хостинг грешил медлительностью для неукраинцев - узкий канал. Тут вроде ровнее.
(Менять айпишник на cssing.iatp.org.ua мне "типа" отказали.) Для переезда использовал мод_реврайт, надеюсь это окажется кому-то полезным.  <!--more-->
<ol class="code">
<li>Options -Indexes +FollowSymLinks</li>
<li>&lt;IfModule mod_rewrite.c&gt;</li>
<li class="tab">RewriteEngine On</li>
<li class="tab">RewriteCond %{HTTP_HOST} cssing\.iatp\.org\.ua$   [NC] </li>
<li class="tab"><del>RewriteRule ^(.*)$  http://cssing.org.ua/$1   [R] </del></li>
<li class="tab">RewriteRule ^(.*)$  http://cssing.org.ua/$1   [R=301,L] </li>
<li>&lt;/IfModule&gt;</li>
</ol>
(<a href="http://lvm.converters.ru/93/ru/article_210.html">позаимствовал</a>)
Можно и более простым способом(спасибо <a href="http://zaartix.ru/">zaARTix</a>):
<ol class="code">
<li>Options -Indexes +FollowSymLinks</li>
<li>&lt;IfModule mod_rewrite.c&gt;</li>
<li class="tab">Redirect permanent / http://cssing.org.ua/</li>
<li>&lt;/IfModule&gt;</li>
</ol>

А работает тут все явно быстрее :). Tnx 2 <strong>Vitos</strong> :).

Просьба всех кто ссылается поменять ссылку на меня в блогроллах - буду возвращать PR...
