---
title: "text-overflow"
date: "2004-08-25"
humanDate: "25 Aug, 2004"
permalink: "2004/08/25/text-overflow/"
tags: 
  - "xhtmlcss"
  - "useful"
comments: 
  -  author: "ganges"
     id: "15"
     url: ""
     date: "2004-08-26 17:06:33"
     humandate: "26 Aug, 2004"
     content: | 
       Есть много друг Горацио такого:
       Не разделяю твой восторг от этого "свойства". Лучше бы ИЕ поддерживал все "вменяемые" properties как-то min-width, например, или псевдокласс :hover - нам бы было счастье ;)

     email: "development@it.net.ua"

  -  author: "akella"
     id: "16"
     url: "http://cssing.iatp.org.ua"
     date: "2004-08-26 19:28:17"
     humandate: "26 Aug, 2004"
     content: | 
       Я просто надеюсь его включат куда нужно...
       Ладно с теми :hover, вот если б он не глючил при первой возможности...
       Вот это было б счастье.:)
       
       <em>поосторожнее с кодировкой</em>

     email: "spin_yura@mail.ru"

  -  author: "alshur"
     id: "393"
     url: "http://htmlcoder.visions.ru/"
     date: "2004-11-21 17:13:03"
     humandate: "21 Nov, 2004"
     content: | 
       всё просто -- <code>text-overflow</code> не входит в w3c css стандарты, вот и не поддерживает его никто, кроме ie

     email: "alshur@narod.ru"

  -  author: "netwizard"
     id: "519"
     url: "http://www.shaftek.org/blog/"
     date: "2005-01-21 09:18:32"
     humandate: "21 Jan, 2005"
     content: | 
       http://www.w3.org/TR/2001/WD-css3-text-20010517/#text-overflow-props

     email: ""

  -  author: "Егоров"
     id: "6631"
     url: "http://new.ukr.net/"
     date: "2006-12-13 18:04:22"
     humandate: "13 Dec, 2006"
     content: | 
       Safari поддерживает text-overflow, также подддерживает opera как -o-text-overflow или около того.
       
       Для мозилки нашел вот такое: 
       http://www.hedgerwow.com/360/dhtml/text_overflow/demo.php

     email: "egor@fine.kiev.ua"

  -  author: "Сергей"
     id: "11996"
     url: ""
     date: "2008-03-17 12:17:14"
     humandate: "17 Mar, 2008"
     content: | 
       Вроде и не очень так полезная статья, а только вспомнился случай один, когда на резиновом сайте клиент вставил ссылку настолько огромную, что в итоге она уехала за границы контентной области. (Не помню, может там даже прокрутка появилась). Тогда думал, как же сделать, чтобы красиво получилось. Сразу же пришла в голову мысль, чтобы сделать красивый переход в самом конце блока, как на Яндексе в почте обрезаются сообщения. Но потом отказался от этой идеи, потому что сложновато там было это реализовать (и времени не много было), поэтому программными средствами там затерли этот момент.
       Но сейчас снова задумался над таким вариантом =)

     email: "zorro-19@yandex.ru"

  -  author: "Сергей"
     id: "11997"
     url: ""
     date: "2008-03-17 13:23:28"
     humandate: "17 Mar, 2008"
     content: | 
       Сделал без графики решение для ИЕ, ФФ и Оперы. Правда меня подловили на том, что если текста мало и он никуда не вылазит, то многоточия быть не должно. =) Я конечно мог бы использовать графику, но в таком случае пришлось бы использовать разные картинки на разном фоне и ещё не рисунок многоточия, а какой-нибудь ПНГ, пореходящим из полупрозрачного в полноцветное изображение. Вот такие соображения =)

     email: "zorro-19@yandex.ru"

  -  author: "Сергей"
     id: "11998"
     url: ""
     date: "2008-03-17 13:28:17"
     humandate: "17 Mar, 2008"
     content: | 
       Ох, не смотря в ссылку как сделать под ФФ сделал похожий вариант =)
       В следующий раз буду внимательнее.

     email: "zorro-19@yandex.ru"

  -  author: "Joni Jones"
     id: "12634"
     url: ""
     date: "2008-06-13 06:27:27"
     humandate: "13 Jun, 2008"
     content: | 
       Очень даже полезное свойство. Использовал его ранее при построении крупных таблиц в одном веб-приложении.

     email: "glushnyov-soft@mail.ru"

  -  author: "all"
     id: "18672"
     url: ""
     date: "2010-05-25 23:25:25"
     humandate: "25 May, 2010"
     content: | 
       http://www.leechy.ru/howto/text-overflow/

     email: "alligator.gav@gmail.com"

layout: "layouts/post.njk"
excerpt: "Интереснейшее свойство нашел. Все наверняка имели дело с обычным <code>overflow</code>, ну или хотя бы слышали. Overflow определяет, что должно происходить с  содержимым блока если оно переполняет его. То есть выходит за пределы этого блока.  Точно так же <code>text-overflow</code> указывает, что произойдет с текстом, когда он переполнит место ему отведенное.
"
---

Интереснейшее свойство нашел. Все наверняка имели дело с обычным <code>overflow</code>, ну или хотя бы слышали. Overflow определяет, что должно происходить с  содержимым блока если оно переполняет его. То есть выходит за пределы этого блока.  Точно так же <code>text-overflow</code> указывает, что произойдет с текстом, когда он переполнит место ему отведенное.
<!--more-->
Вот например такая ситуация:
<pre>
.overflowing{
      border:2px solid #000;
      text-overflow:ellipsis;
      overflow:hidden;
      white-space:nowrap;
      width:256px;/*:)*/
      margin:10px;
      padding:10px;
}
</pre>
(ellipsis в переводе с англ.  &#8212; многоточие)
<div style="text-overflow:ellipsis;border:2px solid #000;overflow:hidden;white-space:nowrap;width:256px;margin:10px;padding:10px;">
Donec non libero. Curabitur metus nulla, fringilla in, mollis eget, condimentum quis, metus. Integer sed arcu quis sem dapibus lacinia. Integer quis felis. Maecenas ac lorem sit amet est congue ornare. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Mauris quis sapien. Integer ipsum. Duis in eros. Aliquam tincidunt cursus wisi. Cras commodo, velit mattis sagittis tincidunt, massa mi consectetuer purus, id malesuada massa mauris sed nulla.
</div>

Как видите достигнув конца блока текст был обрезан.  Казалось бы это и есть свойство <code>overflow</code>, и зачем было выдумывать <code>text-overflow</code>.
Но. 
Это по меньшей мере странно. Но это свойство поддерживает лишь <acronym title="Internet Explorer">IE 6</acronym>.  Когда дело касалось фильтров, порожденных больной фантазией программистов, и поддерживаемых лишь <acronym title="Internet Explorer">IE</acronym> это было нормально. Но этот случай достоин книги рекордов Гинесса, эксплорер <em>поддерживает</em> полезное <acronym title="Cascading Style Sheets">CSS</acronym> свойство, которого <em>не поддерживают</em> Gecko и все остальные.

Но хватит удивлений давайте разберемся, что же оно делает. Если вы посмотрите на эту страничку в  <acronym title="Internet Explorer">IE 6</acronym>. Вы увидите, что там, где во всех броузерах строка была просто обрезана, теперь появилось многоточие &#8212;  "...". Если у вас нет эксплорера значит вам не повезло. Шутка. Вот скрин для тех кто ненавидит его настолько, что не хочет даже запускать:
<img src="http://cssing.org.ua/pic/text-overflow.gif" alt="text-overflow в IE 6" title="text-overflow в IE 6">
Свойство <code>text-overflow</code> может принимать только два значения.
<dl>
<dt><code>clip</code></dt>
<dd>При этом строку постигает обычное обрезание. Как обычный  <code>overflow</code>.</dd>
<dt><code>ellipsis</code></dt>
<dd>А с этим значением мы получаем многоточие при переполнении.</dd>
</dl>

Очень полезным может оказаться это свойство для таблиц.
<pre>
.ovfltable {
	table-layout:fixed;
	border-top: 5px solid #333;
	border-collapse: collapse;
	background: #fff;
	 }
.ovfltable td {
	border-bottom: 1px dashed #333;
	padding: 2px 5px;
	text-overflow:ellipsis;
	overflow:hidden;
	white-space:nowrap;
 } 
</pre>
Вот как это выглядит (best viewed with Internet Explorer 6 :) ):

<table width="350" border="0" cellspacing="0" cellpadding="0" class="ovfltable">
<caption>Пионеры в русском цсс.</caption><colgroup><col width="130" class="col" /><col width="100" /><col /></colgroup>
	<tbody> 
<tr>
		<th>Имя</th>
		<th>Сайт</th>
		<th>Откуда</th>
	</tr><tr><td>Андрей Смирнов</td>
		<td><a href="http://www.ru.id-as.com/" title="id-as.com">www.ru.id-as.com</a></td>
		<td>Россия (Саров?)</td>
	
	<tr>
		<td>Никита Вакорин</td>

		<td><a href="http://www.umade.ru/" title="www.umade.ru">www.umade.ru</a></td>
		<td>Россия</td>
	</tr>
	<tr>
		<td>Denny</td>
		<td><a href="http://www.minimal.ru/" title="www.minimal.ru">www.minimal.ru</a></td>
		<td>Россия</td>

	</tr>
	</tbody>
</table>


Теперь необязательно подгонять ширину ячеек (правда лишь в <acronym title="Internet Explorer">IE 6</acronym>). И по-моему с эстетической точки зрения очень даже смотрится. Когда я вижу многоточие на полуслове сразу понятно что строка обрезана. 

Кстати если попытаться выделить многоточие, то на его месте появляется продолжение строки. Не всей, а той что заменена многоточием.

Вот такое свойство. И очень обидно, что его поддерживает лишь <acronym title="Internet Explorer">IE 6</acronym>. Но надеюсь скоро мозилловцы учтут его.

Кстати если верить этой <a href="http://www.w3schools.com/browsers/browsers_stats.asp">статистике</a>, то IE6 это 70%.

<h3>Еще о том же:</h3>
<ul>
<li><a href="http://www.blooberry.com/indexdot/css/properties/position/textoverflow.htm">Описание</a> <code>text-overflow</code>.</li>
<li><a href="http://www.blakems.com/archives/000077.html">Blakems.com</a>, пост о <code>text-overflow</code>.</li>
<li>На <a href="http://www.google.com/url?sa=U&start=1&q=http://msdn.microsoft.com/workshop/author/dhtml/reference/properties/textoverflow.asp&e=7507">Microsoft</a></li>
</ul>
