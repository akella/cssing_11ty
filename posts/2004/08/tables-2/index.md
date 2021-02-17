---
title: "XHTML таблицы: Добавляем стили"
date: "2004-08-04"
humanDate: "04 Aug, 2004"
permalink: "2004/08/04/tables-2/"
tags: 
  - "xhtmlcss"
  - "design"
  - "perevod"
comments: 
  -  author: "shvets"
     id: "6"
     url: "http://witness.dp.ua"
     date: "2004-08-05 13:59:33"
     humandate: "05 Aug, 2004"
     content: | 
       Попали в лучший сайт Месяца. Поздравляю.

     email: "shvets@iatp.org.ua"

  -  author: "akella"
     id: "7"
     url: "http://cssing.iatp.org.ua"
     date: "2004-08-06 14:37:06"
     humandate: "06 Aug, 2004"
     content: | 
       Это где простите?на иатп?Дайте линк плз,а то моё пребывание в сети стало несколько условным на время...

     email: "spin_yura@mail.ru"

  -  author: "cssing :: Архив   :: XHTML таблицы: Добавляем стили"
     id: "3355"
     url: "http://cssing.org.ua/2004/08/04/tables-2/"
     date: "2006-05-26 10:05:57"
     humandate: "26 May, 2006"
     content: | 
       [...] чика Юрия &#8220;akella&#8221; Артюха. Блог 	Архив 	Ресурсы 	Про это 				 	 XHTML таблицы: Добавляем стили 	D [...]

     email: ""

  -  author: "Дмитрий"
     id: "11849"
     url: ""
     date: "2008-02-22 00:19:50"
     humandate: "22 Feb, 2008"
     content: | 
       интересует внешний отступ границы, от внутренних ячеек и столбцов, чтобы образовалась рамочка похожий аттрибут border-style: double, но при увеличении значинея бордер, увеличиваеться линия, а хотелось бы оставить ееграницы тонкими, как так можна сделать?

     email: "Unregistered@gala.net"

  -  author: "Роман"
     id: "14120"
     url: "http://www.webstarstudio.com"
     date: "2009-02-11 10:40:30"
     humandate: "11 Feb, 2009"
     content: | 
       При увеличении Explorer 7 показывает скрытую таблицу, как этого избежать?

     email: "elkinroma@mail.ru"

layout: "layouts/post.njk"
excerpt: "<strong><a href=\"http://www.snook.ca/archives/000167.html\">Designing Data Part 2: Adding Style</a></strong><br />                        автор: 2004.06.13  &copy; Jonathan Snook <br />                        перевод: 2004.08.04 <a href='/'>Юрий Артюх</a>

Цель этой статьи из двух частей(<a href=\"http://cssing.org.ua/2004/07/31/tables-1/\">первая </a>и <a href=\"http://cssing.org.ua/2004/08/04/tables-2/\">вторая</a>) показать как можно создавать XHTML таблицы и эффективно использовать для них  <acronym title=\"Cascading Style Sheets\">CSS</acronym>.

Во второй части  мы применим стили к структуре документа который мы создали в <a href=\"http://cssing.iatp.org.ua/index.php?p=17\">первой части</a>.
"
---

<strong><a href="http://www.snook.ca/archives/000167.html">Designing Data Part 2: Adding Style</a></strong><br />                        автор: 2004.06.13  &copy; Jonathan Snook <br />                        перевод: 2004.08.04 <a href='/'>Юрий Артюх</a>

Цель этой статьи из двух частей(<a href="http://cssing.org.ua/2004/07/31/tables-1/">первая </a>и <a href="http://cssing.org.ua/2004/08/04/tables-2/">вторая</a>) показать как можно создавать XHTML таблицы и эффективно использовать для них  <acronym title="Cascading Style Sheets">CSS</acronym>.

Во второй части  мы применим стили к структуре документа который мы создали в <a href="http://cssing.iatp.org.ua/index.php?p=17">первой части</a>.
<!--more-->
<h3>Часть 2: Добавляем стили </h3>
<h4>Элемент TABLE </h4>
Что бы как то украсить нашу таблицу я затрону несколько самых важных свойств :
  <code>border</code>, <code>border-collapse</code>, <code>border-spacing</code> и <code>empty-cells</code>.

<h4><code>border</code></h4>

Свойство border аналогично элементу <a href="http://cssing.iatp.org.ua/index.php?p=17#atribut">frame</a> в <acronym title="HyperText Markup Language">HTML</acronym>. Оно задаёт <strong>внешнюю</strong> границу таблицы, но не границу каждой ячейки.

<h4><code>border-collapse</code></h4>

Здесь лишь два значения:: <code>collapse</code> и <code>separate</code>.

При задании collapse, между ячейками нет никакого свободного места. И так как границы между смежными ячейками получаются общие, то есть вероятность, что у нас будет два разных стиля для одной границы. По этому поводу на <acronym title="World Wide Web Consortium">W3C</acronym> есть <a href="http://www.w3.org/TR/CSS21/tables.html#border-conflict-resolution">решение проблемы конфликтования границ</a>, что бы помочь определить какой стиль будет показан. Вот как он выглядит, здесь каждая величина имеет преимущество над нижеследующей.

<ol>
  <li>border-style(стиль границы) для hidden элементов</li>
  <li>border-width (ширина границы)<ol><li>большие значения <ol>
      <li> атрибут rules в <acronym title="HyperText Markup Language">HTML</acronym></li>
      <li>свойство border-width в стилях </li>
      <li> атрибут frame в <acronym title="HyperText Markup Language">HTML</acronym> </li>

    </ol>
  </li>
      <li>меньшие значения    <ol>
      <li> атрибут rules в <acronym title="HyperText Markup Language">HTML</acronym></li>
      <li>свойство border-width в стилях </li>
      <li> атрибут frame в <acronym title="HyperText Markup Language">HTML</acronym> </li>

    </ol>
      </li>
      </ol>
  </li>
  <li>border-style (стиль границы)
    <ol>
      <li>double (двойная)</li>
      <li>solid (обычная)</li>
      <li>dashed (пунктир)</li>
      <li>dotted (точками)</li>
      <li>ridge</li>
      <li>outset</li>
      <li>groove</li>
      <li>inset</li>

    </ol>
  </li>
  <li>элемент
    <ol>
      <li>cell(ячейка)</li>
      <li>row(строка)</li>
      <li>row group(группа строк)</li>
      <li>column(столбец)</li>
      <li>группа столбцов</li>
      <li>таблица</li>
    </ol>
  </li>
  <li>border-style для none </li>
</ol>
Во первых, <acronym title="Internet Explorer">IE</acronym> точно этим правилам <strong>не следует</strong>. Он даёт приоритет границе для всей таблицы над всеми остальными.Он так же воспринимает border-style для hidden, как border-style для none, отдавая преимущество всему остальному. Во вторых, нет никакого правила, какой цвет должен быть у спорной границы.  Таким образом легко можно получить разное отображение под разными броузерами (я получил три разные картинки в броузерах в которых тестировал).

Это не оговорено на <acronym title="World Wide Web Consortium">W3C</acronym>, но я добавил после тестирования в иерархию свойств то что под border-width. 

При раздельной же модели (задано  separate) между границами ячеек есть пространство. Это значение стоит по умолчаниюи скорее всего то, что все привыкли видеть. Что бы увеличить расстояние между ячейками используйте свойство <code>border-spacing</code> property. 

Если задать border-collapse как separate, то Firefox и Opera игнорируют атрибут rules, и я не нашел никакоого стандарта на<acronym title="World Wide Web Consortium">W3C</acronym> который бы описывал это поведение.

<h4><code>border-spacing</code></h4>

Свойство border spacing может быть задано одним или двумя параметрами длины. Если задано одно значение то оно отражается на пространстве во все стороны. При двух значениях, первое отвечает за горизонтальные отступы (слева и справа от ячейки), а второе соответственно за вертикальные. 

Но, как всегда, наш добрый друг <acronym title="Internet Explorer">IE</acronym> не поддерживает свойство border-spacing. Что означает, что мы остаёмcя при использовании старого доброго cellspacing в <acronym title="HyperText Markup Language">HTML</acronym> с тем же результатом. Сразу успокою,  cellspacing все еще входит в <acronym title="Extensible HyperText Markup Language">XHTML</acronym> 1.0 Strict. 

Следует заметить, что цвет который появляется в пространcтве между ячейками, всегда фон таблицы. Задавая background для строк или ячеек вы никогда не измените цвет между ними. 

<h4><code>empty-cells</code><code></code></h4>

Свойство empty-cells принимает два значения: <code>show</code> and <code>hide</code>. И определяет, будет ли видимой граница у пустой ячейки. Его можно так же применить практически к любому элементу таблицы, как для строк, так и для ячеек.

<acronym title="Internet Explorer">IE</acronym>, опять же не поддерживает свойство empty-cells. Это было бы смешно, если б так всех не достало к этому времени. К счастью, есть решение этой проблемы. Просто задайте свойства rules и frames в <acronym title="HyperText Markup Language">HTML</acronym> (описано в <a href="http://cssing.iatp.org.ua/index.php?p=17">первой части</a>). Тогда любая граница примененная к ячейке через <acronym title="Cascading Style Sheets">CSS</acronym> появится.

<h4>Обрабатываем столбцы: COLGROUP и COL </h4>

Эти элементы уникальны в том, что ячейки не наследуют от них свойств. Таким образом только три свойства можно к ним применить: border, background, width и visibility. Эти свойства поддерживаются далеко не полностью, так что будьте готовы!

<h4><code>border</code></h4>

Если применить это свойство для colgroup  правая сторона которого совпадает с границей таблицы, то в Опере она (граница) не будет прорисована. Задавая атрибут border в <acronym title="HyperText Markup Language">HTML</acronym> как 0 или задавая frame как void, мы полностью так же теряем внешнюю границу таблицы.

В Firefox, все работает как и должно. 

В <acronym title="Internet Explorer">IE</acronym>, это свойство не поддерживается. 

<h4><code>background</code></h4>

Это редкий случай, но Firefox единственный кто не поддерживает этого свойства. И Opera и <acronym title="Internet Explorer">IE</acronym> поддерживают. 

<strong>UPDATE:</strong> Firefox 0.9 уже поддерживает это свойство. Ура!

<h4><code>width</code></h4>

Свойство width работает практически идеально во всех броузерах, где я тестировал. Исключение на этот рах составила Опера: для <code>colgroup</code>, она его не поддерживает.

Но надо помнить, что когда свойство width примененл для colgroup, то оно влияет на размер каждого столбца внутри colgroup. К примеру, если задать width 200 пикселов для colgroup содержащей два столбца, то каждый из них будет по 200 пикселов, и всся colgroup 400 пикселов.

<h4><code>visibility</code></h4>

Когда задается для столбца или группы столбцов (colgroup) можно ставить лишь значение <code>collapse</code>. Но ни один из тестируемых не поддерживал это свойство. 

<h3>Выравнивание текста в ячейке</h3>

Есть два свойства в <acronym title="Cascading Style Sheets">CSS</acronym>  которые управляют выравниванием внутри ячейки. Это <code>text-align</code> (атрибут <code>align</code> в <acronym title="HyperText Markup Language">HTML</acronym>)  и <code>vertical-align</code> (атрибут <code>valign</code>). Эти свойства можно применить к любому элементу таблицы, кроме <code>table</code>  и столбцов(<code>colgroup</code> and <code>col</code>) . 

Что бы выравнивать текст в столбце, надо одновременно несколько атрибутов (что бы это работало в большинстве броузеров. Применим <code>align</code> и <code>valign</code> атрибуты в <acronym title="HyperText Markup Language">HTML</acronym> для  тэгов <code>colgroup</code> или <code>col</code>  (это как сказано в первой части не поддерживается Mozilla/Firefox). Нужно еще немного поднапрячься что бы это заработало и там.

<ol>
  <li>Установим <code>id</code> для загодовка столбца. Пример: <code>&lt;th id=&quot;qty&quot;&gt;Quantity&lt;/th&gt;</code></li>
  <li>становим атрибут <code>headers</code> таким же, как и id для столбца того. Пример: <code>&lt;td headers=&quot;qty&quot;&gt;123&lt;/td&gt;.</code> Я не описал эти атрибуты в первой части, так как согласно <acronym title="World Wide Web Consortium">W3C</acronym> они более подходят для accessibility (доступности), которую я не хотел описывать в первой статье.ОднакоБ тут они нам пригодились.</li>

  <li>Теперь используя <acronym title="Cascading Style Sheets">CSS</acronym>, мы можем юзать селекторы для задания стилей. Пример: <code>td[headers=qty] { /*сюда поместить стили*/ } </code>Селектор по атрибуту работает в Mozilla, Firefox, и Opera...но не в <acronym title="Internet Explorer">IE</acronym>. </li>
</ol>

<acronym title="Internet Explorer">IE</acronym> позволяет задавать шрифт и выравнивание на группу столбцов, что вообще говоря не оговорено в рекомендации <acronym title="Cascading Style Sheets">CSS</acronym> .

<h3> Caption (заголовок) </h3>

Caption можно стилизовать как и большинство других блочных элементов, можно использовать выравнивание и настройки шрифтов . Еще одно свойство из<acronym title="Cascading Style Sheets">CSS</acronym> может нам пригодиться: <code>caption-side</code>. Оно может иметь значение top или bottom и позволяет заголовку появляться над или под таблицей соответственно. Firefox пошел даже дальше, он поддерживает значения left и right. Я похож на заевшую пластинку, но <acronym title="Internet Explorer">IE</acronym> не поддерживает <code>caption-side</code>.

<h3>Margins и Padding </h3>

Ячейки не имеют внешних отступов(margins), но имеют внутренние (padding). Вы можете применить margin для таблицы, что отразится на свободном пространстве вокруг неё. Firefox корректно отображал внешний отступ между заголовком и таблицей, тогда как <acronym title="Internet Explorer">IE</acronym> и Opera применили  margin вне заголовка (caption).

<h3>Borders</h3>
Когда вы в режиме separate (ячейки разделены) вы можете менять границы лишь для ячеек и таблицы. Стили для границ строк и столбцов будут проигнорированы. В collapsed режиме и Firefox и Opera позволяют задавать границы для строк и столбцов. <acronym title="Internet Explorer">IE</acronym>  воспринимает режим collapsed  как   separate mode и не позволяет задавать границы для строк и столбцов.

Есть глюк в  Opera,  если у вас есть таблица <code>thead</code>, <code>tbody</code>,
  и <code>tfoot</code> и вы применили стили для границ для <code>thead</code>  тогда они отразятся на верхней части <code>tfoot</code>.И наоборот если зададим для <code>tfoot</code> стиль, то он отразится на <code>tbody</code>.

<h3>Теперь за дело </h3>
Я надеялся остаться максимально информативным и не быть сухим. Я не затронул множество <acronym title="Cascading Style Sheets">CSS</acronym> свойств касающихся текста и селекторов типа 
  <code>:hover</code>. Возможно я дополню свою статью в будущем. 

Оставляю вас с примерами, которые, я надеюсь, вдохновят вас  попробовать что-нибудь новое. Для примеров я пошерстил  web на предмет таблиц данных, и отформатировал по своему.

<ul>
  <li>Посмотрите <a href="http://www.ij-healthgeographics.com/content/3/1/4/table/T1">оригинал</a> , а потом  <a href="/technical/designingdata/example01.html">пример</a>.
  Для этого примера я сохранил форматирование таким же. Оригинал использовал css-заданные тэги font которые конечно были не к месту. Я убрал все форматирующие тэги. Переместил заголовок в caption тэг и использовал <acronym title="Cascading Style Sheets">CSS</acronym> для задания границ. Только это уменьшило общий размер таблицы с 4k до менее чем 1.5k. </li>

  <li>Я взял <a href="http://www.asmusa.org/memonly/asmnews/may99/table1.htm"> еще одну стандартную таблицу</a> и сам её  <a href="/technical/designingdata/example02.html" title="Example Table #2">стилизовал</a>. В этот раз размер с 9k  до 4, в основном только из-за тэгов font. Но я также сэкономил на <code>valign="top"</code> для всех ячеек. С точки зрения стиля я оставил все довольно просто(мне нравится когда все просто(мне тоже - akella)). Я задал первой строке (thead) фон и применил padding для всех ячеек. я использовал атрибуты frame и rules, чтобы создать линии между строками таблицы. То же самон можно было сделать применив границы для ячеек. Последнее, что я сделал&mdashприменил фон (background) первого столбца. Что бы это сделать я добавил некоторые тэги (<code>col</code>) для определения столбцов. Далее я задал класс для первого столбца и фоновый цвет для этого класса.
</li>
</ul>
<h3>Заключение</h3>

<h4>Дополнительная инфа:</h4>
<ul>
<li><a href="http://cssing.iatp.org.ua/index.php?p=17">Украшаем данные часть 1: Структура таблиц</a></li>
  <li><a href="http://www.w3.org/TR/CSS21/tables.html">Раздел таблиц на W3C</a></li>
  <li><a href="http://www.alistapart.com/articles/tableruler/">Линейка для таблиц</a> на A List Apart </li>
  <li><a href="http://www.alistapart.com/articles/zebratables/">Полосатые таблицы</a> на A List Apart </li>

</ul>
<h4>Использованные броузеры:</h4>
<ul>
  <li> <a href="http://www.mozilla.org/products/firefox/">Mozilla Firefox 0.8/0.9</a> </li>
  <li> <a href="http://www.microsoft.com/windows/ie/">Internet Explorer 6.0</a></li>
  <li> <a href="http://www.opera.com/">Opera 7.5</a></li>

</ul>
