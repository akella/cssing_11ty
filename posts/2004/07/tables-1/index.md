---
title: "XHTML таблицы: Структура"
date: "2004-07-31"
humanDate: "31 Jul, 2004"
permalink: "2004/07/31/tables-1/"
tags: 
  - "xhtmlcss"
  - "perevod"
comments: 
  -  author: "shvets"
     id: "4"
     url: "http://witness.dp.ua"
     date: "2004-08-03 15:41:28"
     humandate: "03 Aug, 2004"
     content: | 
       примеры? где примеры? у среднестатистического серфера, на ознакомление с вебстраничкой уходит секунд - 15-20, у меня вообще секунды 4-5. За это время я должен понять, насколько мне информация на ней интересна и буду ли я ее читать сейчас -же или "зайду позже". За это время я не успел отыскать в тексте _жирную_красную_ссылку_ - "Пример1", и не увидел скриншотов/анимаций. Соответсвенно станицу закрыл : ( В остальном, - нормальный перевод.

     email: "shvets@iatp.org.ua"

  -  author: "akella"
     id: "5"
     url: "http://cssing.iatp.org.ua"
     date: "2004-08-03 16:06:10"
     humandate: "03 Aug, 2004"
     content: | 
       большое <strong>спсб</strong> за мнение и здоровую критику. 
       но не стоит опережать события, примеры к этой статье это просто "правильный" код для таблиц.А примеры собственно их стилизации (они наверно имелись ввиду)во второй части статьи, которая этому и посвящена.А здесь хотя и описаны способы изменения их вида, но они касаются HTML кода(они здесь лишь для полноты), что крайне не хотелось бы приводить в качестве примера.
       Но наверно ты прав, надо было сюда хоть какие-то да приткнуть.

     email: "spin_yura@mail.ru"

  -  author: "cssing :: Архив   :: XHTML таблицы: Структура"
     id: "2883"
     url: "http://cssing.org.ua/2004/07/31/tables-1/"
     date: "2006-03-13 15:56:20"
     humandate: "13 Mar, 2006"
     content: | 
       [...] чика Юрия &#8220;akella&#8221; Артюха. Блог 	Архив 	Ресурсы 	Про это 				 	 XHTML таблицы: Структура 	 Designing Da [...]

     email: ""

  -  author: "cssing :: Архив   :: XHTML таблицы: Добавляем стили"
     id: "2884"
     url: "http://cssing.org.ua/2004/08/04/tables-2/"
     date: "2006-03-13 15:56:20"
     humandate: "13 Mar, 2006"
     content: | 
       [...] ok перевод: 2004.08.04 Юрий Артюх Цель этой статьи из двух частей(первая и вторая) показать как можно создавать XHTML таблицы и эффективно использовать для них CSS. 	Во [...]

     email: ""

layout: "layouts/post.njk"
excerpt: "<strong><a href=\"http://www.snook.ca/archives/000164.html\">Designing Data Part 1: Table structure</a></strong><br />                        автор: 2004.06.08  &copy; Jonathan Snook <br />                        перевод: 2004.08.02 <a href='/'>Юрий Артюх</a>
             
Цель этой статьи из двух частей(<a href=\"http://cssing.org.ua/2004/07/31/tables-1/\">первая </a>и <a href=\"http://cssing.org.ua/2004/08/04/tables-2/\">вторая</a>) показать как можно создавать XHTML таблицы и эффективно использовать для них  <acronym title=\"Cascading Style Sheets\">CSS</acronym>."
---

<strong><a href="http://www.snook.ca/archives/000164.html">Designing Data Part 1: Table structure</a></strong><br />                        автор: 2004.06.08  &copy; Jonathan Snook <br />                        перевод: 2004.08.02 <a href='/'>Юрий Артюх</a>
             
Цель этой статьи из двух частей(<a href="http://cssing.org.ua/2004/07/31/tables-1/">первая </a>и <a href="http://cssing.org.ua/2004/08/04/tables-2/">вторая</a>) показать как можно создавать XHTML таблицы и эффективно использовать для них  <acronym title="Cascading Style Sheets">CSS</acronym>.<!--more-->

<strong>Содержание этой статьи (все на этой странице!)</strong>

<ul>
<li><a href="#structura">Структура таблиц</a></li>
<li><a href="#atribut">Атрибуты</a></li>
<li><a href="#conclusion">Заключение</a></li>
</ul>

В первой части рассмотрим базовую структуру таблицы.

<h3 id="structura">Часть 1: Структура таблиц</h3>

Первое дело в написании любой странички это поместить данные в семантический (подходящий по смыслу) и валидный  <acronym title="Extensible HyperText Markup Language">XHTML</acronym>. Давайте начнем с базового примера который вы скорее всего уже использовали.

<pre>&lt;table&gt;
 &lt;tr&gt;
   &lt;th&gt;Year&lt;/th&gt; &lt;th&gt;Quantity&lt;/th&gt;
 &lt;/tr&gt;
 &lt;tr&gt;
   &lt;td&gt;2003&lt;/td&gt; &lt;td&gt;50&lt;/td&gt;
 &lt;/tr&gt;
 &lt;tr&gt;
   &lt;td&gt;2004&lt;/td&gt; &lt;td&gt;100&lt;/td&gt;
 &lt;/tr&gt;
 &lt;tr&gt;
   &lt;td&gt;Total&lt;/td&gt; &lt;td&gt;150&lt;/td&gt;
 &lt;/tr&gt;
 &lt;/table&gt;</pre>

Это простая таблица с 4-мя строками и ячейками первой строки обьявленными как head (заголовочные, просто самая первая строка) . Ничего особенного , но только этот шаг создаёт собственно таблицу.

Далее будем добавлять всякую информацию про таблицу и немного больше конкретизируем строки.

<pre>&lt;table&gt;
 &lt;caption&gt;Total Sales of Thingamajigs&lt;/caption&gt;
 &lt;thead&gt;
 &lt;tr&gt;
   &lt;th&gt;Year&lt;/th&gt; &lt;th&gt;Quantity&lt;/th&gt;
 &lt;/tr&gt;
 &lt;/thead&gt;
 &lt;tfoot&gt;
 &lt;tr&gt;
   &lt;td&gt;Total&lt;/td&gt; &lt;td&gt;150&lt;/td&gt;
 &lt;/tr&gt;
 &lt;/tfoot&gt;
 &lt;tbody&gt;
 &lt;tr&gt;
   &lt;td&gt;2003&lt;/td&gt; &lt;td&gt;50&lt;/td&gt;
 &lt;/tr&gt;

 &lt;tr&gt;
   &lt;td&gt;2004&lt;/td&gt; &lt;td&gt;100&lt;/td&gt;
 &lt;/tr&gt;
 &lt;/tbody&gt;
 &lt;/table&gt;</pre>

Элемент caption (заголовок) описывает таблицу и для чего она вообще нужна. Тэг caption должен быть первым элементом после тэга table  и является заголовком таблицы. В большинстве броузеров этот заголовок будет отображаться сверху по центру таблицы  (над первой строкой) . Во второй части станет ясно как это изменять.

Кроме того мы разделили строки(TR=Table Row) на три группы: THEAD, TFOOT  и TBODY. Но почему же tfoot идёт ПЕРЕД  tbody?А это позволяет , к примеру, броузеру показывать первую строку (head, тэг thead )  и последнюю ( footer, тэг tfoot) , тогда как основная часть таблицы (body, тэг tbody) только загружается (пользователь раньше узнает , что именно показано на таблице).

Теперь мы описали наши TR, время приняться за столбцы. Для этого существует два элемента: COLGROUP (column group) и COL (column). Давайте опять изменим нашу таблицу добавив эту новую информацию.

<pre>&lt;table&gt;
 &lt;caption&gt;Total Sales of Thingamajigs&lt;/caption&gt;
 &lt;colgroup&gt;
 &lt;col /&gt;
 &lt;col /&gt;
 &lt;/colgroup&gt;
 &lt;thead&gt;
 &lt;tr&gt;
   &lt;th&gt;Year&lt;/th&gt; &lt;th&gt;Quantity&lt;/th&gt;
 &lt;/tr&gt;

 &lt;/thead&gt;
 &lt;tfoot&gt;
 &lt;tr&gt;
   &lt;td&gt;Total&lt;/td&gt; &lt;td&gt;150&lt;/td&gt;
 &lt;/tr&gt;
 &lt;/tfoot&gt;
 &lt;tbody&gt;
 &lt;tr&gt;
   &lt;td&gt;2003&lt;/td&gt; &lt;td&gt;50&lt;/td&gt;
 &lt;/tr&gt;
 &lt;tr&gt;
   &lt;td&gt;2004&lt;/td&gt; &lt;td&gt;100&lt;/td&gt;
 &lt;/tr&gt;
 &lt;/tbody&gt;
 &lt;/table&gt;</pre>

Мы указали, что наша таблица содержит одну группу столбцов состоящую из двух столбцов.

<h3 id="atribut">Атрибуты</h3>

Теперь мы вступили на неверную почву. Теоретически большинство атрибутов которые я собиралься описать должны применяться через <acronym title="Cascading Style Sheets">CSS</acronym>. Однако, из-за неправильной поддержки и конфликтования <acronym title="Cascading Style Sheets">CSS</acronym> и <acronym title="HyperText Markup Language">HTML</acronym> для некоторых атрибутов, я опишу их в этой части.

<h4>Атрибуты таблиц: rules (правила), frame (рамка), и border (граница)</h4>
Атрибут border (граница) работает  так же,  как и всегда. Просто задаём числовое значение для указания её ширины  в пикселах. (<a href="http://cssing.iatp.org.ua/examples/tables.html#border">Смотреть пример</a>)

Атрибут frame отвечает за самую  внешнюю границу нашей таблицы. Может принимать такие значения: void, above, below, hsides, vsides, lhs, rhs, box and border. void &mdash; значение по умолчанию, и полностью убирает внешнюю границу таблицы (рамку). Можно почитать на <a href="http://www.w3.org/TR/html4/struct/tables.html#adef-frame">W3C</a> о том как эти значения влияют на отображение таблицы. Отображение границы оказалось разным во всех трёх броузерах <a href="#browsers">в которых я тестировал</a>. <acronym title="Internet Explorer">IE</acronym> прорисовал 3d(обьемную) границу со всех сторон, Opera попросту черную границу, а Firefox серую слева и вверху и черную справа и внизу. Когда в <acronym title="Internet Explorer">IE</acronym> было задано любое значение кроме void, он неверно понимая прорисовывал также границу каждой ячейки. Например, если задать lhs, то  будет прорисована левая граница каждой ячейки. Firefox и Opera прорисовывают в этом случае все правильно. <a href="http://cssing.iatp.org.ua/examples/tables.html#frame">(Смотреть пример)</a>

Атрибут rules имеет пять простых значений: none, groups, rows, cols, and all. Если задано значение none,  то не будет прорисовано никаких линий между ячейками. Это значение задано по умолчанию. Интересно, что если не задать значение этого атрибута (rules), то любой border style (вид границы&mdash;solid,dotted,dashed и т. д.) (заданный через <acronym title="Cascading Style Sheets">CSS</acronym>) для colgroup или col не будет использоваться. Но стоит задать значение none как граница неожиданно возвращается на место. Значение groups задает границу (серую  и разную в <acronym title="Internet Explorer">IE</acronym>, 1px черную в Firefox и Opera) вокруг каждого thead, tfoot, tbody и colgroup. Изменяя значение на rows или cols  прорисует границу между соответственными обьектами. Значение all &mdash; около каждой ячейки. Опять же, <acronym title="Internet Explorer">IE</acronym> выделяется из всех и прорисовывает границу вокруг всей таблицы , если задано любое значение кроме none и атрибут frame не был задан.(<a href="http://cssing.iatp.org.ua/examples/tables.html#rules">Смотреть пример</a>)


Если хотите использовать атрибуты  frame или rules, лучше использовать их вместе.

<h4>Атрибуты столбцов: span, align, valign и width</h4>
К нашим colgroup и col можна применять атрибут span. Это не сливает несколько ячеек в одну, как атрибуты rowspan или colspan atributes для ячеек. Это просто даёт простой путь для задания одного свойства сразу для нескольких столбцов.
<pre>&lt;colgroup&gt;
 &lt;col /&gt;
 &lt;col /&gt;
 &lt;/colgroup&gt;
 &lt;colgroup&gt;
 &lt;col /&gt;
 &lt;col /&gt;
 &lt;col /&gt;
 &lt;/colgroup&gt;</pre>
...можно записать как...
<pre>&lt;colgroup span="2" /&gt;
 &lt;colgroup&gt;
 &lt;col span="2" /&gt;
 &lt;col /&gt;
 &lt;/colgroup&gt;</pre>

Атрибут span для colgroup показывает, что colgroup объединяет (spans) два столбца. Элементы col не используются когда есть атрибут span для colgroup. Если есть элементы col внутри colgroup, то атрибут  span для colgroup игнорируется. Этот атрибут (span) для элемента col показывает наличие 2х столбцов.

Теперь рассмотрим атрибуты align и valign. Их можна применить как к colgroup, так и к col elements, и работают они в основном так же, как и их "ячеечные аналоги". Применяя align="right" для столбца должно задать выравнивание текста по правой стороне для всех ячеек столбца. Эти атрибуты (свойства) важны, так как нет стандартных аналогов в <acronym title="Cascading Style Sheets">CSS</acronym> для того что бы задать text-align (выравнивание текста) для col или colgroup. Таким образом, выравнивание текста должно быть задано на <acronym title="HyperText Markup Language">HTML</acronym> уровне.  К несчастью, Mozilla пока не поддерживает применение этого свойства для colgroup.  <acronym title="Internet Explorer">IE</acronym> поддерживает text-align на <acronym title="Cascading Style Sheets">CSS</acronym> уровне, хотя это и не оговорено в документации на W3C, но лучше придерживаться <acronym title="HyperText Markup Language">HTML</acronym> подхода для лучшей совместимости. 

Атрибут width (ширина) может быть задан в трёх форматах:<br>
  <strong>width="100"</strong> ширина в пикселах<br>
  <strong>width="20%"</strong> ширина в процентах<br>
<strong>width="2*"</strong> относительная ширина, показывающая, что ячейка в 2 раза шире обычной. Относительный способ не работает в <acronym title="Internet Explorer">IE</acronym> и Opera, поэтому его лучше избегать.

Следует помнить так же, что при использовании процентного или относительного метода в <acronym title="Internet Explorer">IE</acronym> делает общую ширину талицы 100%, тогда как  Mozilla и Opera в которых я тестировал, сжимают ширину до минимальной, с наполненными ячейками &#8212; что можно было предвидеть.

Во <a href="http://cssing.iatp.org.ua/index.php?p=18">второй части</a>, мы посмотрим как приукрасить эту таблицу используя <acronym title="Cascading Style Sheets">CSS</acronym>. 

<h3 id="conclusion">Заключение </h3>
<h4>Доступность (accessibility)</h4>

Есть еще один аспект создания хорошей структуры таблицы, который я еще не затронул,  это доступность (accessibility). Это конечно тема которой должна быть уделена отдельная статья. Советую почитать <a href="http://www.w3.org/TR/html4/struct/tables.html#non-visual-rendering">прорисовка таблиц невизуальными методами</a> и <a href="http://www.w3.org/WAI/References/Tablin/">Tablin</a>, метод линеаризации таблиц.

<h4>Примеры</h4>
<ul>
<li><a href="http://cssing.iatp.org.ua/examples/tables.html">Таблицы и атрибуты</a></li>
</ul>
<h3>Дополнительная инфа:</h3>
<ul>
<li><a href="http://cssing.iatp.org.ua/2004/08/04/tables-2/">Украшаем данные часть 2: Добавляем стили</a></li>
  <li><a href="http://www.w3.org/TR/html4/struct/tables.html">Определение таблиц в HTML4.01 Standard</a> (на котором базируется <acronym title="Extensible HyperText Markup Language">XHTML</acronym> 1.0 )</li>

  <li>  <a href="http://www.w3.org/TR/html4/appendix/notes.html#notes-tables">Про таблицы на W3C</a></li>
</ul>
<h3><a name="browsers"></a>Броузеры в которых тестировалось:</h3>
<ul>
  <li>  <a href="http://www.mozilla.org/products/firefox/">Mozilla Firefox 0.8</a></li>
  <li>    <a href="http://www.microsoft.com/windows/ie/">Internet Explorer 6.0</a></li>
  <li>    <a href="http://www.opera.com/">Opera 7.5</a></li>

</ul>
