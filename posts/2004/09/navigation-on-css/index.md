---
title: "Навигация по-русски"
date: "2004-09-01"
humanDate: "01 Sep, 2004"
permalink: "2004/09/01/navigation-on-css/"
tags: 
  - "xhtmlcss"
  - "design"
  - "useful"
comments: 
  -  author: "witness"
     id: "21"
     url: "http://witness.dp.ua"
     date: "2004-09-02 11:51:57"
     humandate: "02 Sep, 2004"
     content: | 
       Классно, есть правда "маленькая" сложность в данной технологии - когда меню генерится движком, то максимум что мы можем получить - это id="current" к активному пункту меню. А конструкция: 
       <code>
       &lt;ul&gt;
       &lt;li&gt;&lt;a href="#" id="n-first"&gt;first&lt;/a&gt;&lt;/li&gt;
       &lt;li&gt;&lt;a href="#" id="n-second"&gt;second&lt;/a&gt;&lt;/li&gt;
       &lt;li&gt;&lt;a href="#" id="n-third"&gt;third&lt;/a&gt;&lt;/li&gt;
       &lt;li&gt;&lt;a href="#" id="n-forth"&gt;forth&lt;/a&gt;&lt;/li&gt;
       &lt;/ul&gt;
       </code>
       вообще нереализуема. 
       
       Что касается еще нереализованных, но безусловно очень интересных технологий в меню:
       <code>&lt;li&gt;&lt;a href="#"&gt;&lt;img src="img24.png (c градиентной прозрачностью)" /&gt;text&lt;/a&gt;&lt;/li&gt;
       &lt;li&gt;&lt;a href="#"&gt;&lt;img src="image24.png" (c градиентной прозрачностью)/&gt;text2&lt;/a&gt;&lt;/li&gt;
       </code>
       
       <code>li a {background: url(1.gif);}
       li a:hover {background: url(2.gif);}</code>
       
       нечто подобное у http://www.blogger.com/start
       но полупрозрачностью там и не пахнет

     email: "shvets@gmail.com"

  -  author: "witness"
     id: "22"
     url: "http://witness.dp.ua"
     date: "2004-09-02 11:53:29"
     humandate: "02 Sep, 2004"
     content: | 
       ой, код не отформатировал : (

     email: "shvets@gmail.com"

  -  author: "akella"
     id: "23"
     url: "http://cssing.iatp.org.ua"
     date: "2004-09-02 12:01:16"
     humandate: "02 Sep, 2004"
     content: | 
       Да это ж я так на скорую руку, я уже почти доделал на CSS полностью. То есть генерировать будет как раз first second и так далее, но задав для каждого BODY свой ID можно будет ВСЮ навигацию переключать из CSS. 
       Было б куда её приставлять там и подогнал бы.
       Главное идея новая , с z-index по-моему еще не игрались в навигациях...
       И главное, что меня в ней беспокоит это читабельность..

     email: "spin_yura@mail.ru"

  -  author: "Yukki Pospel"
     id: "24"
     url: "http://emo.com.ua"
     date: "2004-09-03 10:57:01"
     humandate: "03 Sep, 2004"
     content: | 
       Движок можно пропатчить. Например на ТextPattern мне такое удалось сделать. И по-моему лучше все-таки не id, а class использовать, с точки зрения правильности конструкции.

     email: "creative@emo.com.ua"

  -  author: "akella"
     id: "25"
     url: "http://cssing.iatp.org.ua/"
     date: "2004-09-03 18:54:55"
     humandate: "03 Sep, 2004"
     content: | 
       Могу только добавить, что wordpress просто создан для настройки. Минимум знаний пхп и все. 
       А почему класс? В принципе разницы то никакой. Я исходил из того, что внутри страницы этот АЙДИ встретиться лишь один раз. Но с другой стороны если рассмотреть весь сайт то на каждой странице повториться. Ты это имел виду видимо...
       Тут я с тобой согласен.

     email: "spin_yura@mail.ru"

  -  author: "boffin"
     id: "409"
     url: ""
     date: "2004-12-01 10:17:34"
     humandate: "01 Dec, 2004"
     content: | 
       "...Для такого мелкого разборчивого текста мне пригодились шрифты с сайта dsg4.com..."
       А с поддержкой русских букв, что-нибудь подобное есть?

     email: "oops@iwt.ru"

  -  author: "akella"
     id: "411"
     url: "http://cssing.iatp.org.ua"
     date: "2004-12-01 14:18:39"
     humandate: "01 Dec, 2004"
     content: | 
       Вот вроде тут есть с поддержкой кириллицы.(внизу страницы среди бесплатных)
       http://miniml.com/fonts/.
       Это то что было под рукой, еще найду вышлю, или сюда добавлю.
       Но вообще для себя я подобную проблему решил частичным транслитом. то есть например русская буква Р уже есть и т д.

     email: "akella.a@gmail.com"

  -  author: "boffin"
     id: "415"
     url: ""
     date: "2004-12-02 08:17:43"
     humandate: "02 Dec, 2004"
     content: | 
       to akella
       спасибо, если найдешь не забудь запостить.. :)

     email: "oops@iwt.ru"

  -  author: "Valet - персональный блог, заметки о SEO, жизни и прочей фигне &raquo; Blog Archive &raquo; Хроника ? рика"
     id: "16910"
     url: "http://valetsite.org.ua/krik/xronika-krika/"
     date: "2010-03-03 15:30:58"
     humandate: "03 Mar, 2010"
     content: | 
       [...] О навигации сайта Способ оформления ссылок на сайте Навигация по-русски Навигация вида «Хлебные крошки» - элемент улучшения [...]

     email: ""

  -  author: "cssing :: Архив :: Разделители в меню"
     id: "14990"
     url: "http://cssing.org.ua/2006/11/05/menu-separators/"
     date: "2009-12-09 23:30:47"
     humandate: "09 Dec, 2009"
     content: | 
       [...] &#8220;Навигация по-русски&#8221; - пост двухлетней давности про эту идею [...]

     email: ""

  -  author: "Wad"
     id: "12573"
     url: ""
     date: "2008-06-04 01:06:08"
     humandate: "04 Jun, 2008"
     content: | 
       Идея хорошая с наложением закладок, если учесть что работаешь с бекграундом... а можно ли решить подобную задачу на основе раздвижных дверей... 
       было бы неплохо рассмотреть подобную конструкцию кода, люди помогите я как раз мучаюсь над этой проблемой но пока ничего не получилось...

     email: "wadkorvin@gmail.com"

  -  author: "Леонид"
     id: "14005"
     url: ""
     date: "2009-01-27 19:28:21"
     humandate: "27 Jan, 2009"
     content: | 
       Господа, не подскажете пожалуйста, как сделать меню, открывающееся внутрь экрана на CSS. Меню работает, но с правой стороны при при открытии ссылок, они уходят за предел экрана. Я не большой специалист в этих технологиях. По мере надобности изучаю. Использую свои проги на работе для сотрудников.
       
       Спасибо заранее.

     email: "leonidn@mail.ru"

layout: "layouts/post.njk"
excerpt: "Какое-то время назад мне очень понравились две статьи. Одну написал <a href=\"http://simplebits.com/\">Dan Cederholm</a>, называлась она <a href=\"http://www.simplebits.com/notebook/2003/09/30/accessible_imagetab_rollovers.html\">\"Accessible Image-Tab Rollovers\"</a>,  а вторую  <a href=\"http://nundroo.com/about/\">Didier Hilhorst</a>  и называлась она <a href=\"http://superfluousbanter.org/archives/000186.php\">\"Navigation Matrix\"</a> (и продолжение <a href=\"http://superfluousbanter.org/archives/000187.php\">\"Navigation Matrix Reloaded\"</a>). Обе статьи посвящены построению навигации на базе картинок. 
"
---

Какое-то время назад мне очень понравились две статьи. Одну написал <a href="http://simplebits.com/">Dan Cederholm</a>, называлась она <a href="http://www.simplebits.com/notebook/2003/09/30/accessible_imagetab_rollovers.html">"Accessible Image-Tab Rollovers"</a>,  а вторую  <a href="http://nundroo.com/about/">Didier Hilhorst</a>  и называлась она <a href="http://superfluousbanter.org/archives/000186.php">"Navigation Matrix"</a> (и продолжение <a href="http://superfluousbanter.org/archives/000187.php">"Navigation Matrix Reloaded"</a>). Обе статьи посвящены построению навигации на базе картинок. 
<!--more-->
Второй метод мне не понравился некоторой запутанностью в подсчетах и рисовании этой самой навигации. Хотя конечный визуальный эффект был гораздо лучше, чем в первом. А метод Cederholm'a был практически без недостатков. Вот мне и взбрело в голову их объединить.

А именно я хотел сделать такую же навигацию как сейчас на <a href="http://nundroo.com/">nundroo.com</a>, но по своему. Вот что <a href="http://cssing.org.ua/examples/c3/">получилось</a>.

<h3>XHTML</h3>

Естественно я взял для навигации обычный список. Вот такой:
<pre>
&lt;ul&gt;
&lt;li&gt;&lt;a href='#' id='n-first'&gt;first&lt;/a&gt;&lt;/li&gt;
&lt;li&gt;&lt;a href='#' id='n-second'&gt;second&lt;/a&gt;&lt;/li&gt;
&lt;li&gt;&lt;a href='#' id='n-third'&gt;third&lt;/a&gt;&lt;/li&gt;
&lt;li&gt;&lt;a href='#' id='n-forth'&gt;forth&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;
</pre>

Думаю излишне объяснять почему он лучше всего для этого подходит.

<h3>Графика</h3>

<p style="float:left;"><img style="border:1px solid #ccc;margin:0.5em;padding:3px;" src="http://cssing.org.ua/examples/c3/n-home2.gif" alt="navigation" title="Картинка элемента меню" /> </p>

Картинки, которые я использовал вы можете видеть слева. Для смены изображений я использовал маленький трюк с изменением позиции фона. Это делается что бы избежать мигания при наведении (flicker) и дозагрузки картинок.  Для такого мелкого разборчивого текста мне пригодились шрифты с сайта <a href="http://www.dsg4.com/04/extra/bitmap/index.html">dsg4.com</a>. Как хорошо, что в этом мире есть что то бесплатное.

А это CSS который я использовал для задания фона навигации.
<pre>
 #nav a{
  width:73px;
  background:  url(../n-home.gif) 0 -21px no-repeat;
	}
  #nav #second{
  background:  url(../n-art.gif) 0 -21px no-repeat;
	}
 #nav #third{
  background:  url(../n-arch.gif) 0 -21px no-repeat;
	}
 #nav #forth{
  background:  url(../n-exit.gif) 0 -21px no-repeat;
	}
 #nav #sfirst:hover, #nav #second:hover, 
 #nav #third:hover, #nav #forth:hover{
  background-position: 0 0;
	}
 #nav a#first {
  background-position: 0 0;
	}
</pre>

Тут конечно можно упростить, но не в этом сейчас суть.
Последнее праввило говорит о том, что ссылка #first активная. Разумеется для всей навигации нужно будет написать несколько таких правил.
<h3>CSS</h3>

За основу я взял пример приведенный в статье Cederholm'a. То есть все позиционирование и весь CSS я взял оттуда. Если сейчас посмотреть на то что вышло то мы бы увидели что-то вроде этого:
<img src="http://cssing.org.ua/examples/cutenav/middlenav.gif" alt="navigation" title="Картинка промежуточного результата" />

<h3>Этого мало</h3>

Но мне этого понятно оказалось мало. Хотелось что бы активный элемент навигации находился на переднем плане перекрывая соседних. Да и те в свою очередь перекрывали соседей. Решение пришло само: использовать <code>z-index</code>. И тут моё решение неожиданно усложнилось. Оказывается , <code>z-index</code> <a href="http://www.w3.org/TR/2004/CR-CSS21-20040225/visuren.html#z-index">можно использовать</a> лишь для абсолютно позиционированных блоков. Пришлось добавить такие строки:

<pre>#first{
left:0;
}
#second{
left:63px;
}
#third{
left:126px;
}
#forth{
left:189px;
}
</pre>

Такие рандомные числа я взял не с головы. Просто ширина всех картинок была 73px. Плюс каждую сместил на 10px что бы они пересекались (то чего я так хотел).

Теперь дорога была свободна и я применил <code>z-index</code>:

<pre>
#first{
z-index:13;
}
#second,#third,#forth{
z-index:7;
}
</pre>

Естественно что эту часть я использовал лишь для случая когда активная ссылка #first. Для полноценной навигации нужно будет задать для каждого <code>body</code> свой селектор. Тогда через CSS можно будет доделать навигацию.

А пока можете посмотреть на то что у нас получилось. Вот скриншот:
<img src="http://cssing.org.ua/examples/cutenav/endnav.gif" alt="navigation" title="Картинка конечного  результата" />

<h3>Заключение</h3>

После того как закончил я посмотрел как сделана навигация на nundroo.com. Оказалось там он использовал для свей навигации одну картинку. И соответственно не мог использовать HOVER эффекты. Моя же состоит из нескольких и поэтому в чем то проще для поддержки.  Хотя это и спорный вопрос. В остальном навигация обладает всеми преимуществами CSS. Доступность, мало весит и т д. И неплохо поддерживается в броузерах. Я успел проверить лишь IE 6 и FireFox. И там никаких проблем не было. 

Если вы что-то заметите отзывайтесь в комментарии

Видимо скоро такая навигация появится на этом сайте. Поскольку пиксельные шрифты меня заразили своей ... пиксельностью.

<h3>Результат</h3>

<ul> 
<li><a href="http://cssing.org.ua/examples/c3/">Действуещее меню</a> , которое я сделал (переключаться можно только между первыми двумя элементами,   недостаток времени сказался)
UPDATE: уже работает все.</li>
	<li><a href="http://www.simplebits.com/notebook/2003/09/30/accessible_imagetab_rollovers.html">"Accessible Image-Tab Rollovers"</a>.</li>
<li><a href="http://superfluousbanter.org/archives/000186.php">"Navigation Matrix"</a> </li>
<li><a href="http://superfluousbanter.org/archives/000187.php">"Navigation Matrix Reloaded"</a></li>

</ul>
