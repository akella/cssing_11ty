---
title: "vertical-align:middle"
date: "2005-07-14"
categories: 
  - "xhtmlcss"
  - "useful"
---

Продолжаю традицию обзывать посты экзотическими(для меня) CSS свойствами. Описываю свои трудности с реализацией вертикального выравнивания по центру.

**Update:** рекомендую так же ознакомиться с [новым методом вертикального выравнивания](http://cssing.org.ua/2007/04/26/another-css-valign-method/)

### Одна строка текста - просто

Для того что бы выровнять одну строку например такого кода:

1. <p>
2. Rovno odna stroka texta
3. </p>

Нужен такой CSS:

1. p {
2. line-height:**30px**;
3. height:**30px**;
4. }

Тогда эта строка текста по вертикали будет как раз посередине **p**. Можно посмотреть рабочий пример по адресу [ukr.net](http://www.ukr.net/) (в самом низу, в серой области)

### Несколько строк или просто блочный элемент

Тут все гораздо сложнее. Для начала сформулирую проблему:

1. У нас есть div(или любой блочный элемент) с **известной** высотой
2. Какой-нить абзац текста **P** внутри этого DIVa - известно лишь что он(текст) точно поместится в заданную высоту DIVa
3. Нужно отцентрировать этот текст по вертикали без использования таблиц

Вот такая непростая задачка. Пускай HTML код такой:

1. <div>
2. <p>
3. Because the Welsh and Roman heritage was almost entirely erased by the invasion of low German and then Scandinavian populations....
4. </p>
5. </div>

### Для нормальных броузеров

Для всех броузеров кроме winIE и macIE работает такой CSS код:

1. div {
2. display: table-cell;
3. vertical-align: middle;
4. }

Можно посмотреть мой пример [здесь](http://cssing.org.ua/examples/valign/) - но помните работает только в "нормальных" броузерах (**не ИЕ**).

### для IE

А вот тут начинаются извраты... Изврат **Метод n1**: Стили прямо в коде - внизу ссылка на оригинал с разделением CSS и HTML

1. <div style="display: table; height: 400px; \_position: relative; overflow: hidden;">
2. <div style=" \_position: absolute; \_top: 50%;display: table-cell; vertical-align: middle;">
3. <p style=" \_position: relative; \_top: -50%">
4. any text<br />
5. any height<br />
6. any content, for example generated from DB<br />
7. everything is vertically centered
8. </p>
9. </div>
10. </div>

(взято [отсюда](http://www.jakpsatweb.cz/css/css-vertical-center-solution.html)) Метод не самый удачный имхо...

**Метод n2**: Тоже не без извращений смотрим на центрирование во всем окне - [http://www.kriton.de/CSS/zentrieren/alle-zentriert.html](http://www.kriton.de/CSS/zentrieren/alle-zentriert.html) (видели ID на немецком? - посмотрите! :)) Тот сайт пока умер - смотрим и читаем тут - http://www.umade.ru/log/2004/10/46.html. (не совсем отвечает постановке задачи, но очень распространенная проблема)

**Метод n3**(ИМХО самый удачный и универсальный из тех что я знаю): Метод однако требует добавления в код пустого DIV или другого элемента. Итак центрируем #valign-center:

1. <div class="wrap">
2. <div class="valign-center">
3. <p>lenzi, e profondissima quiete</p>
4. <p>infinito silenzio a questa voce vo comparando: </p>
5. </div>
6. <div class="just-for-IE"></div>
7. </div>

И теперь центрируем для всех нормальных через **`display: table-cell;vertical-align: middle;`**, а для ИЕ используем извраты с `height:100%;` и `display: inline-block`:

1. .wrap {
2. display: table-cell;
3. vertical-align: middle;
4. width: 100%;
5. height: 401px;
6. }
7. .just-for-IE {
8. display: none;
9. width: 1px;
10. margin-left: -1px;
11. }
12. \* html .just-for-IE, \* html .valign-center {
13. display: inline-block;
14. vertical-align: middle;
15. }
16. \* html .valign-center {
17. width: 100%;
18. }
19. \* html .just-for-IE {
20. height: 100%;
21. }
22. \* html .just-for-IE, \* html .valign-center {
23. display: inline;
24. }

Вот такой, мягко говоря немаленький, CSS и то ужатый(не считаю нужным поддерживать IE5Mac). Полную и рабочую версию можно посмотреть [здесь](http://cssing.org.ua/examples/valign/index1.html)

**n4**:способ с помощью expression, смотрите в новом посте [Еще один способ вертикального выравнивания в CSS](http://cssing.org.ua/2007/04/26/another-css-valign-method/).

### Вывод

Если **очень хочется**(выровнять по центру), то **можно**. И даже будет работать - главно в хаках потом не запутаться... Пока писал, думал - сча пару изящных хаков в две строки - нифига.... :( Ну зато хоть есть откуда передирать теперь.

### Инфо

- [Еще один способ вертикального выравнивания в CSS](http://cssing.org.ua/2007/04/26/another-css-valign-method/)
- [Vertical Centering in CSS](http://www.jakpsatweb.cz/css/css-vertical-center-solution.html)
- [Centering (horizontally and vertically) an image in a box](http://www.brunildo.org/test/img_center.html)
- [Вертикальное центрирование](http://www.umade.ru/log/2004/10/46.html)
- [CSS Vertical Centering](http://www.brunildo.org/test/vertmiddle.html)
- [The Underscore Hack](http://wellstyled.com/css-underscore-hack.html)
- [Cross-browser method of centering images](http://mrclay.org/web_design/centered_image/)
