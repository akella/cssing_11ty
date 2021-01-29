---
title: "display:table"
date: "2005-07-03"
categories: 
  - "xhtmlcss"
---

До недавнего времени считал это свойство практически бесполезным. Подходящим лишь для игр с CSS в топ-броузерах. А на самом деле это свойство решило проблему нерешаемую практически никаким другим способом.

### Проблема

К примеру есть на сайте набор вот таких блоков: картинка + заголовок + выдержка. В коде соответственно имеем:

1. <div class="post">
2. <img src="./i/image.jpg" alt="" />
3. <h2><a href="#">Heading</a></h2>
4. <p>text tex text text text text ext text text textt</p>
5. </div>

Cуть проблемы в том что заказчик хочет картинку с одной стороны блока и текст с другой. И это при том что картинка может быть какого угодно размера. Итак первое и очевидное сделать **float:left;** картинке. Выйдет такое.

![FF](http://cssing.org.ua/images/ff.jpg)

Some kind of Heading

Some text. Dean then started to talk about the power of the enclosure element in RSS 2.0. What is great about it is that it enables one to syndicate all sorts of digital content. One can syndicate video, music, calen it is that it enables one to syndicate all sorts of digital content. One can syndicate video, music, calen Some text. Dean then started to talk about the power of the enclosure element in RSS 2.0.

Но заказчик ой как **не хочет что бы текст оказывался под картинкой.** Если бы знать размеры картинок - можно бы было задать ширину для выдержки и заголовка. Но в том то и дело что картинки эти могут быть **какими угодно.**

Вот эту ситуацию я и считал практически нерешабельной в "стандартах" (без таблиц).

### Решение

А решение оказалось таким же простым как и неочевидным. (спасибо [Gunlaug Sørtun](http://www.gunlaug.no/)) Вот недостающий кусок CSS: (для выдержки что загибалась под картинку)

1. div.post p{
2. **display: table;**
3. **\_height: 0;**/\*это для ИЕ5-6\*/
4. **zoom: 1;**/\*это для ИЕ7\*/
5. }

В результате вышеуказанный пример превращается в такой

![FF](http://cssing.org.ua/images/ff.jpg)

Some kind of Heading

Some text. Dean then started to talk about the power of the enclosure element in RSS 2.0. What is great about it is that it enables one to syndicate all sorts of digital content. One can syndicate video, music, calen it is that it enables one to syndicate all sorts of digital content. One can syndicate video, music, calen Some text. Dean then started to talk about the power of the enclosure element in RSS 2.0.

Оттестировано на Opera 7-8, Firefox 1.0, Safari 1.2.4, IE/win. Остались только Unix+Linix броузеры и Ie5Mac. Но и там по идее все идеально.

**Так как ИЕ7 не понимает хак \_height:0 то для него следует использовать либо [conditional comments](http://cssing.org.ua/2005/11/11/ie-magic/) либо другие виды хаков как то - $height. Спасибо Max за замечание!**

Зато теперь какого бы размера ни была картинка - текст всегда будет отображен в стороне от неё.

Говоря русским языком свойство **display:table** обеспечивает **"вертикальную целостность блока"** или **запрет на обтекание FLOATов**. Текст внутри блока с этим свойством не будет обтекать float элементы.

Если кто то знает еще что то касательно этого свойства буду рад услышать.

### Еще немного инфы

- [Pup's Float Hack](http://www.pupinc.com/files/test/float.html) - CSS игры на эту тему
- [Развитие темы + display: table-cell; и т д](http://css.weblogsinc.com/entry/1234000890022801/)
