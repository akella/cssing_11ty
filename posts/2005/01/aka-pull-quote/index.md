---
title: "Цитаты aka Pull Quote"
date: "2005-01-19"
humanDate: "19 Jan, 2005"
permalink: "2005/01/19/aka-pull-quote/"
tags: 
  - "xhtmlcss"
  - "useful"
comments: 
  -  author: "cssing :: Архив   :: cssing 2005"
     id: "2674"
     url: "http://cssing.org.ua/2005/12/27/cssing-highlights-2005/"
     date: "2005-12-27 14:57:12"
     humandate: "27 Dec, 2005"
     content: | 
       [...] просто подборка не самых плохих моих материалов 2005 года. Посты 	 	Цитаты aka Pull Quote - о том как делать красивые блоки с выделением важных частей текста - без л [...]

     email: ""

  -  author: "akella"
     id: "6236"
     url: "http://cssing.org.ua"
     date: "2006-10-22 14:06:37"
     humandate: "22 Oct, 2006"
     content: | 
       Спасибо - все поправил...

     email: "akella.a@gmail.com"

  -  author: "zhulanov"
     id: "6234"
     url: "http://bezdar.ru"
     date: "2006-10-22 13:50:35"
     humandate: "22 Oct, 2006"
     content: | 
       ссылки на примеры битые, на старый сайт указывают :)

     email: "zhulanov@gmail.com"

layout: "layouts/post.njk"
excerpt: "Очень мне нравится идея так называемых \"Pull Quote\". На русском просто цитата или врезка.  Что это такое вы можете посмотреть например на сайте <a href=\"http://www.melos.com.ua/\">http://www.melos.com.ua/</a> . Это те серые цитаты слева.
Вот и решил посвятить им пост.
"
---

Очень мне нравится идея так называемых "Pull Quote". На русском просто цитата или врезка.  Что это такое вы можете посмотреть например на сайте <a href="http://www.melos.com.ua/">http://www.melos.com.ua/</a> . Это те серые цитаты слева.
Вот и решил посвятить им пост.
<!--more-->
<h3>Про это</h3>
Хотя некоторые спорят насчет их полезности мне все же они кажутся очень удобными. Обычно они дублтруют какую-то строку из текста, для лучшего восприятия. Часто это означает и дублирование этой строки в коде. Вот это мне и не нравится. 
Я нашел 2 метода избежания этой ситуации. Вдруг кому пригодятся
<h3>Метод первый</h3>
Первый метод я "спер" с сайта <a href="http://digital-web.com/">http://digital-web.com/</a>.
(например в этой <a href="http://digital-web.com/articles/web_design_for_all_the_senses/">статье</a> - цитата на сером фоне).
Небольшой скрипт решает простую задачу. Однако у них предусмотрено лишь одна такая цитата. И каждый раз в конкретном месте страницы(мы задаём номер абзаца). Для того чтобы скрипт работал нужно
<ol>
<li>Подключить его.</li>
<li>Иметь <code>SPAN</code> с классом <code>pullquote</code></li>
</ol>
В результате скрипт при загрузке спродуцирует такой код:
<pre>
&lt;blockquote class='pullquote'&gt;
  &lt;p class='pullquote'&gt;
    &lt;span class='pullquote'&gt;
        content
    &lt;/span&gt;
  &lt;/p&gt;
&lt;/blockquote&gt;
</pre>
Из которого вы уже можете сделать все что вам прийдет в голову с помощью CSS.(<a href="http://cssing.org.ua/examples/pullquote/wdpull.php" title="Пример украденный из журнала Digital Web">посмотреть пример</a>).
Лучше им конечно не пользоваться - он писался специально для тех страниц. Им нужны была лишь одна цитата.

<h3>Метод второй</h3>
Прочитал в статье "<a href="http://www.fiftyfoureleven.com/sandbox/weblog/2004/jun/javascript-pullquote/">Create a Pull Quote with Javascript (and CSS)</a>". 
Этот метод гораздо универсальнее. С помощью этого скрипта этих цитат вы можете сделать столько сколько <code>SPAN</code> с классом <code>pullquote</code>, причем каждая цитата будет напротив своего "родного" параграфа. 
Требования к работе точно такие, как и у предыдущего.
Этот скрипт будет при загрузке генерировать вот такой код:
<pre>&lt;blockquote class='pullquote'&gt;
  &lt;p&gt;
    &lt;span class=''&gt;
      content
    &lt;/span&gt;
  &lt;/p&gt;
&lt;/blockquote&gt;</pre>
Этот скрипт и меньше и универсальнее.  Им я и рекомендую вам пользоваться.
(<a href="http://cssing.org.ua/examples/pullquote/" title="Универсальный пример">посмотреть пример</a>)
<h3>В конце</h3>
Мне нравится когда с содержанием можно вот так кратко ознакомиться в  таких цитатах. (если их умело подбирать, конечно). А скрипты эти более чем просты в использовании.  Так что себе наверно я такие сделаю, как только перейду на новый <a href="http://wordpress.org/nightly/">WP</a>.  ;)

Вот два примера(скрипты можно легко из них достать)
<ul>
<li><a href="http://cssing.org.ua/examples/pullquote/" title="Универсальный пример">Универсальный пример</a></li>
<li><a href="http://cssing.org.ua/examples/pullquote/wdpull.php" title="Пример украденный из журнала Digital Web">Пример украденный из журнала Digital Web</a></li>
</ul>
