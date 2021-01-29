---
title: "Wordpress и подсветка навигации"
date: "2005-03-28"
categories: 
  - "wordpress"
---

Делюсь своим недавним простым, но все же полезным решением проблемы подсветки навигации, типа "я тут". По крайней мере вкупе с этим строить сайты на базе Wordpress, именно сайты, а не блоги, может оказатсья проще. Вобщем ближе к делу.

### В чем проблема?

Например у вас есть блог на ВП, а теперь вы решили создать кроме главной( она же блог), еще пару статичных страниц (или не очень статичных). Вот как у меня например. Создал я "Про это", "Ресурсы" и "Архив". Резонно было бы после всего этого сделать навигацию между этими разделами сайта.

Сделать это раз плюнуть - навигация то не меняется от страницы к странице. Но тут как всегда приходит мысль о подсветке нужного раздела. То есть если вы на главной в навигации выделяется меню "Блог", и в таком роде. Вот тут и появляется маленькая проблемка.

### Решение

Решение чрезвычайно простое. Даже название решение - это громко сказано. :) Короче говоря. Так как я использую систему темплейтов для своего сайта. ( разложенный на мелкие куски макет странички сайта ) то все изменения коснулись лишь файла **header.php**.

### Определение положения

Для того что бы знать какой элемент навигации подсветить нужно знать где мы находимся. Вот такой простой код помогает и лечит от всех проблем:

1. if(is\_home()) {
2. $homid=" id="current"";
3. }
4. if(is\_archive() || is\_single()) {
5. $arcid=" id="current"";
6. }
7. if(is\_page('Стоит посетить')) {
8. $resid=" id="current"";
9. }
10. if(is\_page('Про это')) {
11. $aboid=" id="current"";
12. }

названия функций говорят сами за себя. Каждая определяет находимся ли мы на главной, на странице с одним постом или же в архиве, и конечно не на странице ли мы с названием...

### Навигация

Ну а теперь дело за малым собственно навигация начинает выглядеть примерно так

1. <ul>
2. <li><a href="/"**<?=$homeid;?>**\>Блог</a></li>
3. <li><a href="/archive/"**<?=$arceid;?>**\>Архив</a></li>
4. <li><a href="/resources/"**<?=$resid;?>**\>Ресурсы</a></li>
5. <li><a href="/about/"**<?=$aboid;?>**\>Про это</a></li>
6. </ul>

Вот и все. Теперь `id="current"` будет у той странички на которой мы находимся. Остальное дело стилей. Как раз на моём блоге работает примерно такая схема.