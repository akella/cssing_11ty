---
title: "5 советов верстальщику"
date: "2008-05-21"
categories: 
  - "xhtmlcss"
  - "common"
---

Принимаю [всеобщее](http://uggallery.audiopeace.ru/2008/05/19/5-advices) [увлечение](http://blog.sribna.com/5-sovetov-verstalschiku.htm) рекомендациями по вёрстке. Мои 5 советов верстальщику. Не тайные манускрипты, а всего лишь простые советы :) Я в этом блоге только тем и занимаюсь, что пытаюсь дать полезные советы, потому слегка повторюсь.

### 1\. Правильная замена на картинки

Заменяйте текст на картинки хорошими CSS-техниками, например, для кликабельного логотипа сайта, нужен такой html:

1. <h1><a href="#">Вау! Я логотип!<span></span></a></h1>

CSS:

1. h1 a{
2. width:250px;height:50px;
3. overflow:hidden;
4. display:block;
5. position:relative;
6. }
7. h1 a span{
8. position:absolute;
9. width:250px;height:50px;
10. top:0;
11. left:0;
12. background:transparent url(../img/kartinka.png) no-repeat 0 0;
13. }

### 2\. Использовать табуляцию в CSS

Суть в табулировании селекторов в зависимости от иерархии. Чем более "глубокий" элемент — тем большим кол-вом табов он будет отделен. Это на любителя, но попробовать совершенно точно стоит. Живой пример этого видно чуть выше, а вот так это выглядит издалека и вживую:

![табулияция в CSS](http://cssing.org.ua/pic/tabsbabs.png)Мне нравится. Как видно, иногда я пишу правила в одну строку, особенно когда подряд идут несколько правил с указанием лишь background

### 3\. Выделенный текст

Очень простой и маленький приём. Иногда полезен. Вот такой код:

1. <h2><span>Ищу ту, особенную!</span></h2>

В дизайне дано такое:

![выделенный текст](http://cssing.org.ua/pic/50c1.png)Выделенный красным "маркером" текст

Если попробовать решать задачу "в лоб", пишем такое:

1. h2 span{background:red;padding:4px;}

получаем это:

![выделенный текст](http://cssing.org.ua/pic/50c2.png)Вторая строка "прилипает" к краю. Мелочь, а неприятно

Вариантов решения несколько, наиболее простой таков:

1. h2{**border-left:4px solid red**;}
2. h2 span{background:red;padding:4px 4px 4px **0**;}

Результат:

![выделенный текст](http://cssing.org.ua/pic/50c1.png)Правильно выделенный текст

Я ранее решал этот вопрос повторением фонового рисунка и паддингом для H2. Подсказал [genn](http://mega.genn.org).

### 4\. Относитесь к вёрстке с чувством юмора

Например, можно давать смешные названия классам и айди. Не стоит этим злоупотреблять, и использовать на сайтах где важна оптимизация, но на сайте какой-то веб-студии, или чисто представительском сайте это вполне оправдано:

1. <div class="i-was-born-in-1494">

Или

1. <div class="usually-i-dont-use-such-a-long-names-for-classes-but-today-is-a-special-day">

Могут сильно повеселить программистов и любителей заглянуть в ваш код. Смешной селектор может быть и коротким, главное, остроумным.

Желательно конечно, чтобы такой класс или айди встречался в коде лишь один раз. Впрочем, возможны варианты. :) Еще можно шутить прямо в CSS.

### 5\. Доводите вёрстку до конца

Никогда не сдавайтесь на пол-пути в сложном проекте. Какими бы титаническими ни были усилия они практически всегда окупаются, если не деньгами то опытом и выносливостью. А так же духом победителя.

### \_\_END\_\_

Адресую [Виталию Харисову](http://harisov.livejournal.com/), [Александру Шабуневичу](http://www.aether.ru/), [Вадиму Макишвили](http://makishvili.ya.ru/), [Владимиру Агафонкину](http://mourner.livejournal.com/).

### Все советы

- [Александр RMcreative Макаров](http://rmcreative.ru/blog/post/neskolko-sovetov-verstalschikam)
- [Павел Коноплицкий](http://www.amazedev.com/5-sovetov-verstalshhiku/)
- [Владимир Mourner Агафонкин](http://habrahabr.ru/blog/webdev/43163.html)
- [Виталий Харисов](http://harisov.livejournal.com/105323.html)
- [Никита Селецкий](http://seleckis.lv/journal/css/5-sovetov-verstalschiku)
- [Александр Исаков](http://uggallery.audiopeace.ru/2008/05/19/5-advices)
- [Алекс Iline](http://www.alexilin.ru/5-sovetov-po-html-i-css/)
- [Александр Шабуневич](http://www.aether.ru/blog/2008/06/04/5-advices)
- [Юрий Дроздов](http://blog.sribna.com/5-sovetov-verstalschiku.htm)
- [The Webmakers Lounge](http://www.webmakerslounge.com/news/work-advices/)
- [Engelside](http://engelside.net/5-for-coder/)
- [Марат Таналин](http://tanalin.com/blog/2008/05/xhtml-css-coding-tips-n-tricks/)
- [Вадим Макеев](http://pepelsbey.net/2008/05/soviet-country/)
- [Юрий Артюх](http://cssing.org.ua/2008/05/21/5-things-to-remembe/)
- [Павел Корнилов](http://lusever.livejournal.com/21502.html)
- [kizu.ru](http://kizu.ru/webdev/five-tips/)
