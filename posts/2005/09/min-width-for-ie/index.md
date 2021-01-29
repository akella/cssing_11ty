---
title: "min-width для IE"
date: "2005-09-02"
categories: 
  - "xhtmlcss"
  - "useful"
---

Два**Три** способа как это можно сделать в ИЕ...

### min-width по нормальному

Это очевидно, так **должно** быть, это должно работать:

1. #min-width {
2. min-width:600px;
3. }

Но, как вы можете легко догадаться, работает везде, кроме чего? Правильно! Интернет Эксплорера! :)

### Вступление

Здесь и дальше я буду укрощать(задавать минимальную ширину) блок **#min-width**.

### Метод 1: JavaScript

Вот такой простенький кусок CSS (перемешанного с JS) решает проблему..

1. #min-width {
2. min-width:800px;
3. width:expression(document.body.clientWidth < 770? "770px": "auto" );
4. }

Или так например:

1. \* html #min-width {
2. width:expression(document.body.clientWidth > 770? "100%" :"770px");
3. }

[смотреть пример](http://cssing.iatp.org.ua/examples/min-width/min1.html) Одна из проблем с этим методом описана ниже - заголок ВАЖНО!

- [max-width in Internet Explorer (min-width)](http://www.svendtofte.com/code/max_width_in_ie/)

### ВАЖНО

Однако помните, что первый метод при некоторых Доктайпах вызывает подвисание IE WinXP SP1 при ресайзах окон. Смена доктайпа и еще пару примочек помогает. Например переход XHTML на HTML спасает. Вот тут читайте подробнее - [min-width, max-width re-hacked](http://blog.unmatchedstyle.com/hacks/min-width-max-width-re-hacked).

### Метод второй: два обертывающих DIV

Этот метод потребует добавления в код двух дополнительных DIV. Примерно так:

1. <div id="min-width">
2. <div class="minwidth">
3. <div class="container">
4. tut ku4a texta
5. </div>
6. </div>
7. </div>

Тогда вот такой CSS нам сымитирует min-width для IE:

1. /\*для всех броузеров что понимают min-width \*/
2. #min-width {
3. width:50%;
4. min-width:400px;
5. }
6. /\* для IE \*/
7. \* html .minwidth {
8. border-left:400px solid #fff;/\*min-width\*/
9. position:relative;
10. float:left;
11. z-index:1;
12. }
13. \* html .container {
14. margin-left:-400px; /\*-min-width\*/
15. position:relative;
16. float:left;
17. z-index:2;
18. }

[смотреть пример](http://cssing.iatp.org.ua/examples/min-width/min.html) Если вкратце: то внутрь блока помещают другой, с границей равной минимальной ширине. Который и не дает ИЕ сжимать этот блок. Более подробное описание:

- [min-width for IE](http://www.cssplay.co.uk/boxes/minwidth.html)
- [How to Use CSS to Solve min-width Problems in Internet Explorer](http://www.webreference.com/programming/min-width/)

### **Update:** Метод 3: JavaScript

Для простоты приводимого кода я сделаю min-width для тэга body. Если необходимо реализовать для какого то блока - достаточно задать ID и использвать getElemetById.

Вобщем достаточно проинклюдить в страницу вот такой скрипт:

1. var d = document;
2. var winIE = (navigator.userAgent.indexOf("Opera")==-1 && (d.getElementById && d.documentElement.behaviorUrns)) ? true : false;

4. function bodySize(){
5. if(winIE && d.documentElement.clientWidth) {
6. sObj = d.getElementsByTagName("body")\[0\].style;
7. sObj.width = (d.documentElement.clientWidth<**760**) ? "**760px**" : "**100%**";
8. }
9. }

11. function init(){
12. if(winIE) { bodySize(); }
13. }
14. onload = init;
15. if(winIE) { onresize = bodySize; }

В принципе аналогично первому методу с ескпрешонами - но этот вариант исключает подвисание броузера при ресайзе - поэтому если уж бить джаваскриптом, то лучше этим - хотя за определение броузера стыдно - но такова селяви... (подсмотрено живьем [тут](http://digital-web.com/))

### Заключение

В очередной раз убеждаемся что заставить ИЕ понимать можно все. Но не всегда это очевидно и стоит того.

### Все ссылки

- [min-width, max-width re-hacked](http://blog.unmatchedstyle.com/hacks/min-width-max-width-re-hacked)
- [max-width in Internet Explorer (min-width)](http://www.svendtofte.com/code/max_width_in_ie/)
- [min-width for IE](http://www.cssplay.co.uk/boxes/minwidth.html)
- [How to Use CSS to Solve min-width Problems in Internet Explorer](http://www.webreference.com/programming/min-width/)
