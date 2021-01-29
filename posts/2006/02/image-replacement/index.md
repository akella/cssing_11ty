---
title: "Некоторые техники замены текста картинками (image replacement)"
date: "2006-02-23"
categories: 
  - "xhtmlcss"
  - "design"
---

Обзор некоторых способов замены текста картинками.

### Зачем?

Часто хочется чтобы заголовки были красивыми, и не хочется себя ограничивать парой тройкой шрифтов пользователя (из тех что есть у всех) — тут и приходят на помощь способы заменить этот текст (оставить его в коде для поисковиков и других юзер агентов) на картинки или флэш. Итак для начала заменяем такой код на картинку:

1. <h1>Заголовок - картинка</h1>

### 1\. Способы без добавления HTML

Именно их я, как правило, и использую, если не нужно сильно заморачиваться на поддержке браузерами. Самые популярные: **1.** LIR ([пример](http://www.moronicbajebus.com/playground/cssplay/image-replacement/) ) (так же известен как Phark Method)

1. h1{
2. text-indent: -9000px;
3. overflow: hidden;
4. height:80px;width:200px;
5. background-image: url("img.gif");
6. }

Этот первый я чаще всего и применяю. Хотя при отключенных картинках мы не увидим ничего :(. Руководствуюсь принципом: «нефиг». :)

**2.** Метод Leahy/Langridge ([подробнее](http://www.kryogenix.org/code/browser/lir/))

1. h1{
2. padding: 80px 0 0 0;
3. overflow: hidden;
4. background-image: url("img.gif");
5. height: 0px !important; /\* для большинства броузеров \*/
6. height /\*\*/:80px; /\* для блочной модели IE5.5 \*/
7. }

Вместо 80px естественно нужно вставить свою высоту.

**3.** MIR (Malarkey Image Replacement) ([подробнее](http://www.stuffandnonsense.co.uk/archives/mir_image_replacement.html))

1. h1{
2. letter-spacing :-1000em;
3. height:80px;width:200px;
4. background-image: url("img.gif");
5. }

Довольно изящный метод. Все три разумеется при отключенных картинках не покажут ничего. Следует это помнить. Доступность страдает, но иногда бывают ситуации в которых эти методы могут сильно выручить. [Смотреть пример.](http://cssing.org.ua/examples/ir/)

### 2\. Способы c добавлением HTML

**1.** Метод Pixy ([подробнее](http://wellstyled.com/css-replace-text-by-image.html)) **HTML:**

1. <h1>Заголовок - картинка<span></span></h1>

**CSS:**

1. h1{
2. margin:0; padding:0;
3. position:relative;
4. width:200px; height:80px;
5. overflow:hidden;
6. }
7. h1 span {
8. display:block;
9. position:absolute; left:0; top:0; z-index:1;
10. width:200px; height:80px;
11. background:url("img.gif") top left no-repeat;
12. }

Если картинки отключены текст будет видно. Один из лучших методов, главное не забыть вставить спан. По сути фоновая картинка ложится сверху на текст и при ее отсутствии текст просвечивает. Есть еще несколько вариаций которые работают в тех же браузерах (ИЕ 5 и выше и все остальные более или менее новые) но отличаются немного структурой кода: [Levin Alexander's](http://levin.grundeis.net/files/20030809/alternatefir.html) например. **2.** Thierry Image (re)Placement ([подробнее](http://www.tjkdesign.com/articles/tip.asp)) **HTML:**

1. <h1><img src="pic.gif" />Заголовок - картинка</h1>

**CSS:**

1. h1 {
2. height:80px;
3. width:200px;
4. overflow:hidden;
5. position:relative;
6. }
7. h1 img {
8. z-index:1;
9. position:absolute;
10. top:0;
11. left:0;
12. }

### Другие способы

Среди прочих нельзя не упомянуть [sIFR](http://www.mikeindustries.com/sifr/) (и [неофициальные апгрейды](http://www.maratz.com/blog/archives/2006/01/16/multi-color-sifr-201/) к нему) — замена с помощью флеша и джаваскрипта. И некоторые методы замены картинками еще на сервере: [Dynamic Text Replacement](http://www.alistapart.com/articles/dynatext) и на русском [PHP+CSS: Динамичеcкая замена текста](http://www.umade.ru/log/2006/01/167.html). А так же то, к чему мы прийдем рано или поздно :), CSS3 метод замены текста:

1. h1 {
2. content: url(img.gif);
3. }

Ну или простой и банальный font-face, который наконец заработает везде.

### Ссылки

Собственно не такой же ж я умник что бы самому вот это все придумать. :) К тому же это далеко не полный список методов, лишь те, которые я практикую и считаю удобными для себя.

- [Мои примеры - для теста](http://cssing.org.ua/examples/ir/)
- [Revised Image Replacement](http://www.mezzoblue.com/tests/revised-image-replacement/)
- [CSS Image Replacement and Alternatives to CSS Image Replacement](http://css-discuss.incutio.com/?page=ImageReplacement)

Линков из этих двух страничек хватит всерьез и надолго :) С названиями полная путаница, поэтому называл я по имени того кто выше в гугле. Хоть для какой то ориентации.
