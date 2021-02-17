---
title: "CSS print framework"
date: "2008-04-07"
humanDate: "07 Apr, 2008"
permalink: "2008/04/07/css-print-framework/"
tags: 
  - "xhtmlcss"
  - "useful"
comments: 
  -  author: "Эд"
     id: "14703"
     url: "http://agorod.org.ua/"
     date: "2009-08-14 20:10:12"
     humandate: "14 Aug, 2009"
     content: | 
       "Просто экономлю мировую энтропию, чтобы кто-то не парился и украл у меня этот файл. =)"
       Уважаю :)
       Файл действительно помог, спасибо (хотя я конечно не делаю 10 сайтов в неделю =)

     email: "ederlondsy@ya.ru"

  -  author: "Евгений"
     id: "12199"
     url: "http://designformasters.info"
     date: "2008-04-07 19:35:22"
     humandate: "07 Apr, 2008"
     content: | 
       Если в тексте много ссылок получается нечитабельно, а ведь печатают часто для того чтобы читать было удобнее.
       
       Можно полечить так http://designformasters.info/posts/improving-link-display-for-print/, жаль только требуется JS, можно, конечно, и на сервере сгенерить сноски, но поисковики это не оценят (а может им и все равно).
       
       У меня на сайте сделано как раз как описано в той статье.

     email: "evgeniy.dfm@gmail.com"

  -  author: "Никита Васильев"
     id: "12198"
     url: "http://elv1s.ru/"
     date: "2008-04-07 19:30:51"
     humandate: "07 Apr, 2008"
     content: | 
       URL в скобочках для IE:
       
       a {filter: expression(runtimeStyle.filter = '', 
       this.appendChild(
       		document.createTextNode(' ('+this.href+') ')
       	)
       )}
       
       Получите, распишитесь.

     email: "me@elv1s.ru"

  -  author: "Никита Васильев"
     id: "12200"
     url: "http://elv1s.ru/"
     date: "2008-04-07 20:03:56"
     humandate: "07 Apr, 2008"
     content: | 
       Наврал я. Не работает. Скобки портят всё, пришлось их убрать. Вот тут рабочий пример: http://elv1s.ru/files/js/ie-content-after.html

     email: "me@elv1s.ru"

  -  author: "Ante"
     id: "12201"
     url: ""
     date: "2008-04-07 20:53:19"
     humandate: "07 Apr, 2008"
     content: | 
       http://npj.ru/seminar/printversion/
       старое доброе

     email: "antejan@gmail.com"

  -  author: "akella"
     id: "12203"
     url: "http://cssing.org.ua"
     date: "2008-04-08 01:33:06"
     humandate: "08 Apr, 2008"
     content: | 
       Спасибо Никита, спасибо Ante, спасибо Евгений! Добавил линки в пост. Ситуация с кучей ссылок в посте, имхо, конечно редкая, но решение просто суперское! 
       
       Я если честно против этих хаков для ИЕ, и джаваскриптов. Это из серии 30килобайтовый джаваскрипт эмулирующий CSS3... В фреймворк &#8212; лучше не добавлять :). Я очень ценю простоту. Но на живых проектах, да, нужно, не поспоришь. Все же склонен рассматривать это (ссылки в скобочках) как мелкую приятность =)
       
       Впрочем, это лишь моё мнение.
       
       PS: Классный сайт и проекты, Никита! =)

     email: "akella.a@gmail.com"

  -  author: "Никита Васильев"
     id: "12204"
     url: "http://elv1s.ru/"
     date: "2008-04-08 10:19:53"
     humandate: "08 Apr, 2008"
     content: | 
       Спасибо, Юрий!
       
       Я так и не понял как скормить IE круглые скобки. Однако квадратные «[]» он съел.

     email: "me@elv1s.ru"

  -  author: "Junior"
     id: "12217"
     url: "http://mordovorot.ru/"
     date: "2008-04-08 19:42:48"
     humandate: "08 Apr, 2008"
     content: | 
       Отличный обзор, добавлю в закладки.
       
       Я часто применяю классы для подготовки страницы для печати. На макетах бывает множество элементов которые печатать не нужно. Поэтому на этапе разметки кода (или постпроцессом) каждому такому элементу ставим класс .noprint а в стилях пишем .noprint {display: none;}. Таким образом мы избавляемся от перечисления ID элементов или прочих селекторов.
       
       В качестве особо продвинутой техники можно произвести расстановку класса .nopda совместно с классом .noprint. Бывает, что в версии для PDA нужны некоторые элементы, которые отключены в версии для печати (навигация, например), но при этом некоторые элементы все же надо отключить. И комбинированием свойст для этих двух классов добиваемся нужного состава страниц.
       
       Вот как-то так. :)

     email: "webware@bk.ru"

  -  author: "c0nst"
     id: "12218"
     url: "http://www.javenue.info"
     date: "2008-04-08 19:51:00"
     humandate: "08 Apr, 2008"
     content: | 
       Юрец, это ты был вдохновлен моим опен-сорсным начинанием? 
       Кстати, мне для проекта нужнен был простенький css-framework. Хотел сначала typography скачать, но теперь выбор очевиден.

     email: "glad2cu@gmail.com"

  -  author: "Vasily Polovnyov"
     id: "12243"
     url: ""
     date: "2008-04-10 00:40:50"
     humandate: "10 Apr, 2008"
     content: | 
       А ещё полезно и логично убирать вообще все формы form{display: none}

     email: "vast@whiteants.net"

  -  author: "akella"
     id: "12244"
     url: "http://cssing.org.ua"
     date: "2008-04-10 00:45:10"
     humandate: "10 Apr, 2008"
     content: | 
       Спасибо Василий! Отличный совет, добавил во фреймворк убирание форм..

     email: "akella.a@gmail.com"

  -  author: "Волошин Сергей"
     id: "12264"
     url: "http://svoloshyn.org.ua/"
     date: "2008-04-16 10:16:21"
     humandate: "16 Apr, 2008"
     content: | 
       Никита Васильев,
       кажется я смог решить проблему с круглыми скобками, вот демка:
       http://svoloshyn.org.ua/lab/ie-content-after2.html
       
       <code>a {background-image:expression(
       this.runtimeStyle.backgroundImage = 'none',
       	this.appendChild(
       		document.createTextNode(' ' + String.fromCharCode(40) + this.href + String.fromCharCode(41) + ' ')
       	)
       )}</code>
       
       ссылка по теме: http://www.developers.org.ua/archives/zerkella/2007/11/07/specsimvoli-v-javascript/

     email: "svoloshyn@gmai.com"

  -  author: "Никита Васильев"
     id: "12278"
     url: "http://elv1s.ru"
     date: "2008-04-18 10:20:57"
     humandate: "18 Apr, 2008"
     content: | 
       Сергей, спасибо! 
       
       Так и знал, что копать надо в эту сторону.

     email: "me@elv1s.ru"

  -  author: "Максим"
     id: "12411"
     url: "http://savepic.info"
     date: "2008-05-14 01:28:13"
     humandate: "14 May, 2008"
     content: | 
       Мне понравилось! А главное, все очень просто ;) Спасибо за файлик!

     email: "most2wanted@gmail.com"

  -  author: "Луч Надежды"
     id: "12426"
     url: "http://www.ln-tlt.ru"
     date: "2008-05-19 10:21:39"
     humandate: "19 May, 2008"
     content: | 
       Спасиб. Познавательно.

     email: "aaa@ln-tlt.ru"

  -  author: "Сергей"
     id: "12456"
     url: "http://www.zabirai.ru"
     date: "2008-05-22 22:39:55"
     humandate: "22 May, 2008"
     content: | 
       Отличный шаблончик! Обязательно пригодится.

     email: "zabirai@mail.ru"

  -  author: "бизнес-план"
     id: "12433"
     url: "http://www.bishelp.ru"
     date: "2008-05-19 23:12:01"
     humandate: "19 May, 2008"
     content: | 
       Очень полезно для начинающих типа меня, спасибо за пост!

     email: "bishelp@list.ru"

  -  author: "Vladimir"
     id: "12657"
     url: "http://blog.sjinks.org.ua/"
     date: "2008-06-17 06:48:44"
     humandate: "17 Jun, 2008"
     content: | 
       Akella, спасибо за идею... Почему же я раньше до этого не додумался? :-)
       
       Один вопрос: разве Юзверь-Агент не будет игнорировать margin у body? Ведь в CSS 2.1, если я не ошибаюсь, для этих целей элемент @page?

     email: "sjinks@sjinks.org.ua"

  -  author: "akella"
     id: "12658"
     url: "http://cssing.org.ua"
     date: "2008-06-17 08:33:17"
     humandate: "17 Jun, 2008"
     content: | 
       Гм, ну на данный момент не игнорирует =). А о том что должен, я честно говоря и не знал :-[
       
       Рад что знания оказались полезными!

     email: "seijuro@yandex.ru"

  -  author: "Принтер тоже Веб-дизайн."
     id: "13146"
     url: "http://softwaremaniacs.org/forum/web/3449/"
     date: "2008-08-26 13:15:58"
     humandate: "26 Aug, 2008"
     content: | 
       [...] http://cssing.org.ua/2008/04/07/css-print-framework/ [...]

     email: ""

  -  author: "Пингвин"
     id: "13153"
     url: "http://spamparampampam.com/"
     date: "2008-08-28 19:48:49"
     humandate: "28 Aug, 2008"
     content: | 
       Прекрасный блог, прошу вас и дальше писать столь интересно и вразмутельно. Сейчас сам захотел заняться парой проектов - не простое это дело, уходит все свободное время.

     email: "ping2@mail.ru"

layout: "layouts/post.njk"
excerpt: "Пафосное название для моего обычного стандартного print.css который я всюду инклюдю.
"
---

Пафосное название для моего обычного стандартного print.css который я всюду инклюдю.
<!--more-->
Несколько общих правил для печатных стилей, которые будет легко дополнить своими. 

Разумеется, по-хорошему, каждый проект нуждается в своем печатном стиле. Но, на деле, когда вы верстаете 10 (вы монстр!) сайтов в неделю, такой вот шаблон print.css становится приятным бонусом, и знаком вашего профессионализма.

Файл состоит из нескольких условных групп правил. Сложного нет ничего. Просто экономлю мировую энтропию, чтобы кто-то не парился и украл у меня этот файл. =)
<h3>Общие стили</h3>
Шрифты и цвета. При печати лучше смотрится черный на белом, и текст с засечками:
<ol class="code">
<li>body {</li>
<li class="tab">margin:.2in .55in; <small>/*отступы от края страницы, для красоты*/</small></li>
<li class="tab">padding:0;</li>
<li class="tab">background:#fff;</li>
<li class="tab">color:#000;</li>
<li class="tab">font:12pt "Times New Roman", Garamond, serif;<small>/*шрифт с засечками*/</small></li>
<li class="tab">}</li>
<li>form, <br />#secondary, <br />#sidebar,<br /> #nav,<br /> #whatever {<small>/*прячем ненужные при печати блоки, единственная часть печатного файла которую нужно обновлять на новом проекте*/</small></li>
<li class="tab">display:none; </li>
<li class="tab">}</li>
</ol>
В каждом проекте свои блоки нужно скрывать и показывать, все же остальные правила остаются неизменными.
<h3>Текст</h3>
Самые обычные приятные отступы и размеры. h1 самый большой, h2 поменьше, h3 еще меньше. И все прижимаются к тексту (margin-bottom:0):
<ol class="code">
<li>h1, h2, h3 {</li>
<li class="tab">margin:.6em 0 0 0;</li>
<li class="tab">font-family:Georgia,Serif;</li>
<li class="tab">font-weight:normal;</li>
<li class="tab">clear:both;</li>
<li class="tab">}</li>
<li>h2 {</li>
<li class="tab">font-size:240%;</li>
<li class="tab">margin:.3em 0 0 0;</li>
<li class="tab">}</li>
<li class="tab">...</li>
<li>h3+blockquote,<br /> h2+blockquote,<br /> p+ul{ <small>/*между заголовком и абзацем лучше иметь минимальный отступ*/</small></li>
<li class="tab">margin-top:.2em;</li>
<li class="tab">}</li>
</ol>
<h3>Ссылки</h3>
Псевдоселектор <code>:after</code>, работает только в "хороших" броузерах. В результате, в печати после текста ссылки добавляет её URL в скобочки.
<p class="img con"><img src="http://cssing.org.ua/pic/url.png" alt="УРЛ в скобочках" /><span>URL</span></p>
Вот, css-magic:
<ol class="code">
<li>#content a[href]:after {</li>
<li class="tab">content: " (" attr(href) ") ";</li>
<li class="tab">font-size: 90%;</li>
<li class="tab">}</li>
<li>#content a[href^="/"]:after{<small>/*для ссылок вроде href="/feed/"*/</small></li>
<li class="tab">content: " (http://cssing.org.ua/" attr(href) ") ";</li>
<li class="tab">}</li>
<li>abbr:after,<br />
acronym:after {<small>/* аббревиатуры */</small></li>
<li class="tab">content: " ("attr(title)") ";</li>
<li class="tab">}</li>
</ol>
<h3>Результат</h3>
Этих стилей достаточно, чтобы ваша страничка начала печататься примерно так:
<p class="img con"><a href="http://cssing.org.ua/pic/cssing.pdf"><img src="http://cssing.org.ua/pic/cssingprint.png"  alt="скриншот версии для печати" /><span>Версия для печати (pdf, 160Kb)</span></a></p>
Мне, очень нравится.
Все что нужно дальше, легко добавить в этот фреймворк. Но базу он задает. Обожаю маленькие фреймворки!
<h3>Читать дальше</h3>
<ul>
<li><a href="http://cssing.org.ua/pic/print.css">Мой CSS print фреймворк</a> (осторожно! размер файла 1.3Kb)</li>
<li><a href="http://www.alistapart.com/stories/goingtoprint/">CSS Design: Going to Print</a></li>
<li><a href="http://www.digital-web.com/articles/css_styling_for_print_and_other_media/">CSS Styling for Print and Other Media</a></li>
<li><a href="http://www.smashingmagazine.com/2007/02/21/printing-the-web-solutions-and-techniques/">Printing the Web: Solutions and Techniques</a></li>

<li><a href="#">На New York Times, кстати продают <a href="http://www.nytimes.com/2008/04/07/world/middleeast/07iraq.html?_r=1&hp=&oref=slogin&pagewanted=print">места в печатной версии</a> (вверху справа) :) </a></li>
<li><a href="http://cssing.org.ua/wp-content/themes/cssing2/css/print.css">Печатные стили для CSSing</a> &#8212; типичный пример моего фреймворка в работе, добавлено несколько специфических правил для блога</li>
<li><a href="http://npj.ru/seminar/printversion/">Подбор материалов c семинара npj</a> &#8212; очень всеобъемлющий материал, несмотря на возраст.</li>
<li><a href="http://designformasters.info/posts/improving-link-display-for-print/">Javascript для вынесения ссылок из текста в конец печатной версии</a></li>
<li><a href="http://elv1s.ru/files/js/ie-content-after.html">Замена :after для IE (expression), нюанс &#8212; нет скобочек</a></li>
</ul>

Буду рад если поделитесь своими советами и печатными хаками. С радостью внесу в этот файл, чтобы он был еще более полезным!
