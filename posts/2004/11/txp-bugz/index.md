---
title: "Разборки с TXP"
date: "2004-11-03"
humanDate: "03 Nov, 2004"
permalink: "2004/11/03/txp-bugz/"
tags: 
  - "blogging"
  - "useful"
comments: 
  -  author: "Yukki Pospel"
     id: "95"
     url: "http://blog.emo.com.ua"
     date: "2004-11-04 19:57:50"
     humandate: "04 Nov, 2004"
     content: | 
       На самом деле можно использовать кастомный вывод статей используя секции, или через плагины по алтернативному выводу статей. Патчить код - последнее дело :)

     email: "creative@emo.com.ua"

  -  author: "akella"
     id: "96"
     url: "http://cssing.iatp.org.ua"
     date: "2004-11-04 20:10:00"
     humandate: "04 Nov, 2004"
     content: | 
       Это как? Я просто еще не совсем разобрался с ТХР...
        У меня просто не отображались секции вообще. Все отображалось только на одной странице.
       
       Ну и если уж код глючный так править его святое дело. :)

     email: "spin_yura@mail.ru"

  -  author: "Yukki Pospel"
     id: "99"
     url: "http://blog.emo.com.ua"
     date: "2004-11-05 16:03:42"
     humandate: "05 Nov, 2004"
     content: | 
       Каждой секции задает страница, которая будет отображать контент в ней. Это в разделе Sections.
       
       А вывод статей используя нужную секцию можно так
       <txp:article_custom form="full" section="blog" />

     email: "creative@emo.com.ua"

  -  author: "Yukki Pospel"
     id: "100"
     url: "http://blog.emo.com.ua"
     date: "2004-11-05 16:06:32"
     humandate: "05 Nov, 2004"
     content: | 
       Скушали теги :) сорри
       
       txp:article_custom form="full" limit="1" section="blog" sortby="Posted" sortdir="desc"

     email: "creative@emo.com.ua"

  -  author: "akella"
     id: "101"
     url: "http://cssing.iatp.org.ua"
     date: "2004-11-05 16:08:32"
     humandate: "05 Nov, 2004"
     content: | 
       Это понятно.
       Просто я <strong>не мог</strong> попасть на страницу соответствующую секции articles например. 
       <strong>Все отображалось</strong> на "Default template"

     email: "spin_yura@mail.ru"

  -  author: "Yukki Pospel"
     id: "281"
     url: "http://blog.emo.com.ua"
     date: "2004-11-09 20:29:00"
     humandate: "09 Nov, 2004"
     content: | 
       Так ты и скажи, что дело в ошибке в исходниках :) а то "я не смог" - я уж подумал, что у тебя не получалось :)
       А вообще, TXP 1.0rc весьма богат могучими багами: не работает удаление статей, добавление линков, ошибки с секциями и так далее. Хотя на большее число уже поправили код - так что наипервейшая задача выкачать последний вариант TXP с багтрека.

     email: "creative@emo.com.ua"

  -  author: "edgy"
     id: "395"
     url: "http://edgy.ru/"
     date: "2004-11-25 08:45:28"
     humandate: "25 Nov, 2004"
     content: | 
       >выкачать последний вариант TXP с багтрека
       это где?

     email: "i@edgy.ru"

  -  author: "Yukki Pospel"
     id: "396"
     url: "http://blog.emo.com.ua"
     date: "2004-11-25 16:30:59"
     humandate: "25 Nov, 2004"
     content: | 
       http://dev.textpattern.com

     email: "creative@emo.com.ua"

  -  author: "Yurik"
     id: "1552"
     url: ""
     date: "2005-04-23 16:22:53"
     humandate: "23 Apr, 2005"
     content: | 
       вот тут на русском подробно расписано - как, где и откуда производить выкачивание последней версии техтпатеррна
       http://www.textpattern.ru/forum/viewtopic.php?id=2

     email: "httptextpattern.ru"

layout: "layouts/post.njk"
excerpt: "Начал было разбираться с TXP. И застопорился на одном моменте. Этот пост вряд ли будет много значить для тех кто не пользовался textpattern'ом
"
---

Начал было разбираться с TXP. И застопорился на одном моменте. Этот пост вряд ли будет много значить для тех кто не пользовался textpattern'ом
<!--more-->
<h3>Проблема</h3>
Никак не мог заставить работать секции. Все посты <strong>всегда</strong> отображались только с помощью так называемого "Default page template". Что я только не делал. переключал все возможные варианты работы clean URLs и messy. Ничего не помогло. Что бы я не делал индивидуальные посты всегда отображались на "Default page template".

<h3>Решение</h3>
Решение оказалось совсем не очевидным, но принесло надежду (я уж думал что я совсем туп). Вот что нужно делать если вы вдруг будете испытывыть подобную проблему с этой CMS (этот баг вроде только в последней версии от 20 сентября).

Необходимо исправить в файле pubslish.php в 55 строке такой код:
<pre>
$s = (empty($s)) ? 'default' : $s;
</pre>
На такой 
<pre>
$s = (empty($s)) ? '' : $s;
</pre>
То есть попросту удалить слово default. После этого у меня сразу заработали секции так как я хотел. 
В оригинале эту маленькую хитрость можно прочитать <a href="http://forum.textpattern.com/viewtopic.php?id=3950#28968">тут</a>.
