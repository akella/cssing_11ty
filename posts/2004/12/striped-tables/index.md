---
title: "Таблицы в полоску"
date: "2004-12-13"
humanDate: "13 Dec, 2004"
permalink: "2004/12/13/striped-tables/"
tags: 
  - "xhtmlcss"
  - "useful"
comments: 
  -  author: "DpakoH"
     id: "573"
     url: ""
     date: "2005-02-02 15:08:33"
     humandate: "02 Feb, 2005"
     content: | 
       http://cssing.iatp.org.ua/examples/melos/table.html
       не работает в опера 8 beta

     email: "dpakoh13@gmail.com"

  -  author: "CB&#8217;s blog  &raquo; Полосатые таблицы"
     id: "4281"
     url: "http://sudoku.org.ua/rus/blog/2006/02/17/striped-tables/"
     date: "2006-08-12 23:50:47"
     humandate: "12 Aug, 2006"
     content: | 
       [...] Внимательный читатель сразу же может заметить мол сколько можно, тема раскрыта и точка, надоели повторы, практически то же самое скорее всего можно почитать тут (en), тут (рус) и тут (рус), а также додуматься самому при возникновении необходимости в сабже. Но я считаю, что соотношения пользы нижеизложенного кода к размеру в байтах так велико, что лучше прочитать еще раз, выучить наизусть, найти все баги, и в конце-концов повесить в рамочку под стеклом. Javascript now works [...]

     email: ""

  -  author: "Человек"
     id: "154666"
     url: ""
     date: "2013-07-06 12:02:02"
     humandate: "06 Jul, 2013"
     content: | 
       Если зрить в DOM, то баловать с CSS вообще не нужно.
       А тем более если ресурс чужой. И править много чего не получиться.
       
       function stripe(id) {
        var table = document.getElementById(id);
        if (! table) { return; }
        var trs = table.getElementsByTagName('tr');
        for (var i = 0; i &lt; trs.length; i += 2) {
        trs[i].style.backgroundColor=&quot;rgb(204, 204, 204)&quot;;
        }
        }
       мне хватает букмарклета под FF для однотипных задач как ваша.
       javascript:(
       function(){
       for(var i=0;i&lt;document.body.childNodes[1].children[2].rows.length;i+=3){
        document.body.childNodes[1].children[2].rows[i].style.backgroundColor=&quot;rgb(204,204,204)&quot;;
       }
       })()

     email: "sekret@prism.ru"

layout: "layouts/post.njk"
excerpt: "Давненько уже на <a href=\"http://www.alistapart.com/\" title=\"A List Apart\">ALA</a> была статья про <a href=\"http://www.alistapart.com/articles/zebratables/\">\"Полосатые таблицы\"</a>. Решил поделиться маленькой хитростью которую подсмотрел там же в обсуждении статьи.
"
---

Давненько уже на <a href="http://www.alistapart.com/" title="A List Apart">ALA</a> была статья про <a href="http://www.alistapart.com/articles/zebratables/">"Полосатые таблицы"</a>. Решил поделиться маленькой хитростью которую подсмотрел там же в обсуждении статьи.
<!--more-->
<h3>Что было</h3>
В оригинальной статье использовался довольно немаленький (по меркам современного веба) скрипт. Этот скрипт  искал таблицу и потом определенным ячейкам присваивал фоновый цвет. 
Причем этот скрипт не работал в старых ИЕ(5.0, 5.5) поскольку они не поддерживали такое присвоение.(у меня по крайней мере не заработало). 

Присвоение же цвета агрументировалось экономией имени класса.(<acronym title="ин май опинион">ИМО</acronym> абсолютно не нужной). перевод статьи можно почитать здесь: <a href="http://cssing.iatp.org.ua/articles/index.php?p=6">Полосатые таблицы</a>
<h3>Другие пути</h3>
Порывшись на ALA в обсуждении этой статьи, я обнаружил несколько намного более изящных путей для решения проблемы.
<h3>Путь первый: универсальный</h3>
Идея первого пути почти такая же в оригинале. Но теперь мы присваиваем не фоновые цвета для каждой ячейки, а классы для строк.
Вот собственно скрипт:
<pre>
function stripe(id) {
    var table = document.getElementById(id);
    if (! table) { return; }
    var trs = table.getElementsByTagName('tr');
    for (var i = 0; i < trs.length; i += 2) {
      trs[i].className += ' even';
    }
  }
</pre>
Где вместо ID нужно подставить ID будущей "зебры".
Лично я,  для раскраски нескольких таблиц, использую такую конструкцию:
</pre><pre>
/*Running onLoad Scripts*/  
  function runScripts()
	{
	stripe('price');
	stripe('price-a');
	stripe('price-b');
	stripe('price-d');
	}
window.onload = runScripts;
</pre>
Ну и естественно, так как скрипт лишь расставляет лишь класс для строк без CSS тут не обойтись:
<pre>
#price tbody tr.even td {
	background-color: #edf3fe
}
</pre>
Таким образом на любой странице этим подключенным скриптом  будут раскрашены таблицы с id <code>price,price-a,price-b,price-d</code>.
Пример можно посмотреть по адресу: <a href="http://cssing.iatp.org.ua/examples/melos/table.html" title="Пример зебры">http://cssing.iatp.org.ua/examples/melos/table.html</a>
<h3>Второй путь: НЕуниверсальный</h3>
Это решение наверно можно назвать реализацией CSS3  в <acronym title="Internet Explorer">ИЕ</acronym>.
Работает это естественно только для ИЕ. :(
Но уж больно симпатичное и изящное оно.
Для полосатых таблиц достаточно добавить в CSS вот такую строку:
<pre>
.zebra tr {
background: expression(this.rowIndex%2 == 1?'#F0F0F0':'#FFF');
} 
</pre>
Все таблицы класса .zebra будут полосаты в ИЕ.
<h3>Само собой</h3>
Для того что бы работал скрипт, надо что бы структура таблиц была примерно такая:
<pre>
&lt;table id='playlist'&gt;
  &lt;tbody&gt;
    &lt;tr class='odd'&gt;
     ...
    &lt;/tr&gt;
  &lt;/tbody&gt;
&lt;/table&gt;
</pre>
Ну и для красоты рекомендую сразу поставить <strong>cellspacing="0"</strong> для всех таблиц которые вам нужны полосатыми.

В обсуждении были еще методы. Но первый был лучшим, а второй занятным.  Что и определило мой выбор.
