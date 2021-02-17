---
title: "Заголовки"
date: "2004-08-11"
humanDate: "11 Aug, 2004"
permalink: "2004/08/11/heading/"
tags: 
  - "xhtmlcss"
  - "design"
layout: "layouts/post.njk"
excerpt: "Заголовки, какие бы они ни были, всегда бросаются в глаза первыми.

<h4><a href=\"http://www.cameronmoll.com/\">www.cameronmoll.com</a></h4>
Эти заголовки просто поразили меня. Скажу честно, я очень удивился когда выделил текст в них. На первый взгляд, да и  на второй это была картинка, но никак не текст!
"
---

Заголовки, какие бы они ни были, всегда бросаются в глаза первыми.

<h4><a href="http://www.cameronmoll.com/">www.cameronmoll.com</a></h4>
Эти заголовки просто поразили меня. Скажу честно, я очень удивился когда выделил текст в них. На первый взгляд, да и  на второй это была картинка, но никак не текст!
<!--more-->
Просто поразительно какое гармоничое слияние нашел дизайнер своего красивого шрифта и обычного текста (курсива).
Когда я начал разбираться, вот какой маленький трюк применил <a href="http://www.cameronmoll.com">Камерон Молл</a>.
Для заголовков он использует такую конструкцию:
<code>&lt;h1&gt;&lt;img class="capA" src="/img/letters/a.gif" alt="" width="50" height="28" /&gt;&lt;span class="hide"&gt;A&lt;/span&gt;LA does it again&lt;/h1&gt;</code>
То есть в заголовке перед первой буквой идет картинка (они хранятся для каждой буквы).  А потом идет сам текст,  причем первую букву он заключил в <code>&lt;span&gt;</code>, что бы она не отображалась. А для каждой буквы-картинки выбрал идеальный правый отрицательный отступ (все разные!). 
Вот как это выглядит:
<pre>
...
.capI {margin-right: -13px; vertical-align: -20%;}
.capL {margin-right: -5px; vertical-align: -20%;}
.capM {margin-right: -16px; vertical-align: -20%;}
.capN {margin-right: -22px; vertical-align: -20%;}
.capO {margin-right: -3px; vertical-align: -20%;}
.capP {margin-right: -14px; vertical-align: -20%;}
.capS {margin-right: -7px; vertical-align: -40%;}
.capT {margin-right: -20px; vertical-align: -20%;}
.capU {margin-right: -9px; vertical-align: -25%;}
...
</pre>
И из-за этого выглядит это все потрясающе. Заголовки смотрятся цельными словами, и курсив Georgia (именно этот шрифт используется для текста) гармонично сливается с красивым шрифтом дизайнера.
Вы можете подумать что наличие  картинки портит вид при чтении без стилей.
Я тоже так подумал. Оказалось совсем нет. Эти буквы настолько красивы (я про первые буквы заголовков), что я даже не обратил на них внимания. Они совсем не мешают читать и не нарушают гармонию странички. Если вам лень загружать всю страницу вот те самые заголовки с сайта <a href="http://www.caneronmoll.com/">CaneronMoll.com</a>:

<div class="alpha-shadow"><div><img alt="Заголовок с сайта Камерон Молла" title="Заголовок с сайта Камерон Молла" width="214" height="67" src="http://cssing.iatp.org.ua/pic/cammol/h1ala.gif" /></div></div>
<div class="alpha-shadow"><div><img alt="Заголовок с сайта Камерон Молла" title="Заголовок с сайта Камерон Молла" width="214" height="67" src="http://cssing.iatp.org.ua/pic/cammol/h1post.gif" /></div></div>
<div class="alpha-shadow"><div><img alt="Заголовок с сайта Камерон Молла" title="Заголовок с сайта Камерон Молла" width="214" height="67" src="http://cssing.iatp.org.ua/pic/cammol/h1simple.gif" /></div></div>
<span class="non">* * *</span>Вобщем я думал описать побольше заголовков, но эта тема оказалась намного интересней, чем я предполагал. Я обязательно посвящу еще несколько постов ей. И надеюсь как-то обобщить всю информацию.
