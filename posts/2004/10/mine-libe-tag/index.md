---
title: "Мой любимый тэг"
date: "2004-10-28"
humanDate: "28 Oct, 2004"
permalink: "2004/10/28/mine-libe-tag/"
tags: 
  - "xhtmlcss"
  - "thoughts"
comments: 
  -  author: "Vova"
     id: "94"
     url: ""
     date: "2004-11-04 14:17:12"
     humandate: "04 Nov, 2004"
     content: | 
       div 
       h1-h6 
       ul
       
       к сожалению в русскоязычном мире все три либо не используются вообще, либо используются не по назначению

     email: ""

  -  author: "witness"
     id: "92"
     url: "http://witness.dp.ua"
     date: "2004-11-04 11:07:09"
     humandate: "04 Nov, 2004"
     content: | 
       a
       p
       img

     email: "shvets@gmail.com"

  -  author: "akella"
     id: "93"
     url: "http://cssing.iatp.org.ua"
     date: "2004-11-04 13:38:21"
     humandate: "04 Nov, 2004"
     content: | 
       a?
       :)
       это наверно самый главный

     email: "spin_yura@mail.ru"

  -  author: "Остап"
     id: "97"
     url: ""
     date: "2004-11-05 02:13:01"
     humandate: "05 Nov, 2004"
     content: | 
       Последнее особенно странно, т.к. DIV - это тег-затычка, который стоит применять только тогда, когда логически адекватного ситуации элемента не подбирается.

     email: "quqlus@mobilemail.ru"

  -  author: "akella"
     id: "98"
     url: "http://cssing.iatp.org.ua"
     date: "2004-11-05 15:59:29"
     humandate: "05 Nov, 2004"
     content: | 
       По крайней мере я так не думаю.
       Пока не появился тэг section (XHTML2) более удачного элемента для группировки или разбития страницы на секции я не вижу.
       Ясно что некоторые его используют часто не к месту. И по многу раз вкладывая... Для них он затычка.
        Для меня же чисто семантическая группировка обьектов.(впрочем как и для w3c)
       Например "sidebar" или "content". Разве в этом случае это затычка? Как еще их сгруппировать?

     email: "spin_yura@mail.ru"

  -  author: "Vova"
     id: "389"
     url: ""
     date: "2004-11-17 11:45:28"
     humandate: "17 Nov, 2004"
     content: | 
       div - единственный контейнер для блочных элементов
       
       а использовать его действительно нужно с чувством меры
       
       смотрите в код и учитесь: верстка на дивах с одним дивом:
       http://www.wwzwickau.de/

     email: ""

  -  author: "Arefiev"
     id: "428"
     url: ""
     date: "2004-12-10 01:45:05"
     humandate: "10 Dec, 2004"
     content: | 
       Можно ли при использовании тега &lt;dl&gt; сделать так что бы термин и определение термина располагались на одной строке.
       Т.е. хочется генерить списки вида:
       Производитель: "Русский продукт"
       Страна производства: Россия
       Размер:30х40х35
       Вес:1,2 кг

     email: "arefiev@gmail.com"

  -  author: "Arefiev"
     id: "429"
     url: ""
     date: "2004-12-10 01:46:18"
     humandate: "10 Dec, 2004"
     content: | 
       я имелл виду тег <code>dl</code>
       (форма вырезала)

     email: "arefiev@gmail.com"

  -  author: "akella"
     id: "431"
     url: "http://cssing.iatp.org.ua"
     date: "2004-12-11 15:43:18"
     humandate: "11 Dec, 2004"
     content: | 
       Для этого удобно применить FLOAT
       то есть к примеру
       dl{width:100px;}
       dt{float:left;width:50px;}
       dd{clear:both;width:50px;margin-left:50px}
       Попробуй так.
       В своей версии ukr.net, в центральной колонке я именно так и поступил. Можешь посмотреть код, я там все закоментировал структурно.

     email: "akella.a@gmail.com"

layout: "layouts/post.njk"
excerpt: "После этого сообщения меня наверно будут считать geek'ом (кто не знает что такое geek, читать <a href=\"http://www.google.com/search?hl=en&lr=&c2coff=1&client=firefox-a&oi=defmore&q=define:Geek\">тут</a>).
Но тем не менее, меня почему то заинтересовал этот вопрос. И я решил сформировать тройку лучших. :)
"
---

После этого сообщения меня наверно будут считать geek'ом (кто не знает что такое geek, читать <a href="http://www.google.com/search?hl=en&lr=&c2coff=1&client=firefox-a&oi=defmore&q=define:Geek">тут</a>).
Но тем не менее, меня почему то заинтересовал этот вопрос. И я решил сформировать тройку лучших. :)
<!--more-->
<h3>Как можно определить лучшего?</h3>

Можно решить, что все теги предназначены для разных целей. И определение лучшего (читай любимого) невозможно. Но лично мне кажется, что очень часто их области применения пересекаются. И несомненно при таком пересечении сказываются наши личные предпочтения. Вот тут то и оказывается, что есть любимчики и ... другие теги.
<h3>Моя тройка</h3>

Недолго думая я определил свою тройку.
<ol>
<li><strong>&lt;dl&gt;</strong></li>
<li><strong>&lt;ul&gt;</strong></li>
<li><strong>&lt;div&gt;</strong></li>
</ol>

Оказалось, два первых места это списки. Легко обьяснимо - любые два куска похожей инфы это уже список.  Тем более для них удобно писать стили.
<strong>&lt;dl&gt;</strong>. Просто он мне нравится. Тем более он несет в себе много смысла, очень гибкого смысла. Например на этом сайте он используется для правой колонки. Каждый заголовок в ней это тег &lt;dt&gt;, а каждый список ссылок содержится в &lt;dd&gt;. Что по-моему  полностью отвечает семантике моеё правой колонки. (&lt;dt&gt; - термин,&lt;dd&gt; - определение термина.)
Примерно так выглядит этот тег без стилей:
<dl>
<dt>Geek</dt>
 <dd>a person who may be very smart yet lacks the social graces of those who are considered cool , a "computer geek" is someone who spends too much time on the computer and has no social life.</dd>
<dd>www.planetpals.com/coolkidz.html</dd>

<dt>Geek 2</dt>
<dd>Deragatory term for a person with limited social skills, and usually strong technical skills. While anybody can become a nerd, geeks are born, not made. The difference between a geek and a dweeb is that dweeb has no redeeming qualities. </dd>
<dd>www.msg.net/kadow/answers/g.html</dd>
</dl>

Код выглядит примерно так (без инфы )
<pre>
&lt;dl&gt;
&lt;dt&gt;&lt;/dt&gt;
  &lt;dd&gt;&lt;/dd&gt;
  &lt;dd&gt;&lt;/dd&gt;
&lt;dt&gt;&lt;/dt&gt;
  &lt;dd&gt;&lt;/dd&gt;
  &lt;dd&gt;&lt;/dd&gt;
&lt;/dl&gt;
</pre>
Почему  <strong>&lt;ul&gt;</strong> занял второе, и так понятно. практически любая навигация (без таблиц) сделана на его основе. И вообще очень удобная штука.
Ну а с <strong>&lt;div&gt;</strong> и так все ясно, куда ж без него?

А ваша тройка? ;-)
