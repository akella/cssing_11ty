---
title: "text-overflow"
date: "2004-08-25"
categories: 
  - "xhtmlcss"
  - "useful"
---

Интереснейшее свойство нашел. Все наверняка имели дело с обычным `overflow`, ну или хотя бы слышали. Overflow определяет, что должно происходить с содержимым блока если оно переполняет его. То есть выходит за пределы этого блока. Точно так же `text-overflow` указывает, что произойдет с текстом, когда он переполнит место ему отведенное. Вот например такая ситуация:

.overflowing{
      border:2px solid #000;
      text-overflow:ellipsis;
      overflow:hidden;
      white-space:nowrap;
      width:256px;/\*:)\*/
      margin:10px;
      padding:10px;
}

(ellipsis в переводе с англ. — многоточие)

Donec non libero. Curabitur metus nulla, fringilla in, mollis eget, condimentum quis, metus. Integer sed arcu quis sem dapibus lacinia. Integer quis felis. Maecenas ac lorem sit amet est congue ornare. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Mauris quis sapien. Integer ipsum. Duis in eros. Aliquam tincidunt cursus wisi. Cras commodo, velit mattis sagittis tincidunt, massa mi consectetuer purus, id malesuada massa mauris sed nulla.

Как видите достигнув конца блока текст был обрезан. Казалось бы это и есть свойство `overflow`, и зачем было выдумывать `text-overflow`. Но. Это по меньшей мере странно. Но это свойство поддерживает лишь IE 6. Когда дело касалось фильтров, порожденных больной фантазией программистов, и поддерживаемых лишь IE это было нормально. Но этот случай достоин книги рекордов Гинесса, эксплорер _поддерживает_ полезное CSS свойство, которого _не поддерживают_ Gecko и все остальные.

Но хватит удивлений давайте разберемся, что же оно делает. Если вы посмотрите на эту страничку в IE 6. Вы увидите, что там, где во всех броузерах строка была просто обрезана, теперь появилось многоточие — "...". Если у вас нет эксплорера значит вам не повезло. Шутка. Вот скрин для тех кто ненавидит его настолько, что не хочет даже запускать: ![text-overflow в IE 6](http://cssing.org.ua/pic/text-overflow.gif "text-overflow в IE 6") Свойство `text-overflow` может принимать только два значения.

`clip`

При этом строку постигает обычное обрезание. Как обычный `overflow`.

`ellipsis`

А с этим значением мы получаем многоточие при переполнении.

Очень полезным может оказаться это свойство для таблиц.

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

Вот как это выглядит (best viewed with Internet Explorer 6 :) ):

<table width="350" border="0" cellspacing="0" cellpadding="0" class="ovfltable"><caption>Пионеры в русском цсс.</caption><colgroup><col width="130" class="col"><col width="100"><col></colgroup><tbody><tr><th>Имя</th><th>Сайт</th><th>Откуда</th></tr><tr><td>Андрей Смирнов</td><td><a href="http://www.ru.id-as.com/" title="id-as.com">www.ru.id-as.com</a></td><td>Россия (Саров?)</td></tr><tr><td>Никита Вакорин</td><td><a href="http://www.umade.ru/" title="www.umade.ru">www.umade.ru</a></td><td>Россия</td></tr><tr><td>Denny</td><td><a href="http://www.minimal.ru/" title="www.minimal.ru">www.minimal.ru</a></td><td>Россия</td></tr></tbody></table>

Теперь необязательно подгонять ширину ячеек (правда лишь в IE 6). И по-моему с эстетической точки зрения очень даже смотрится. Когда я вижу многоточие на полуслове сразу понятно что строка обрезана.

Кстати если попытаться выделить многоточие, то на его месте появляется продолжение строки. Не всей, а той что заменена многоточием.

Вот такое свойство. И очень обидно, что его поддерживает лишь IE 6. Но надеюсь скоро мозилловцы учтут его.

Кстати если верить этой [статистике](http://www.w3schools.com/browsers/browsers_stats.asp), то IE6 это 70%.

### Еще о том же:

- [Описание](http://www.blooberry.com/indexdot/css/properties/position/textoverflow.htm) `text-overflow`.
- [Blakems.com](http://www.blakems.com/archives/000077.html), пост о `text-overflow`.
- На [Microsoft](http://www.google.com/url?sa=U&start=1&q=http://msdn.microsoft.com/workshop/author/dhtml/reference/properties/textoverflow.asp&e=7507)
