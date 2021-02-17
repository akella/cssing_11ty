---
title: "Слепая доступность"
date: "2016-12-26"
humanDate: "26 Dec, 2016"
permalink: "2016/12/26/blind-accessibility/"
tags: 
  - "web-standards"
  - "thoughts"
comments: 
  -  author: "Подборка статей, переводов, докладов и ресурсов для Frontend-разработчика | Библиотека программиста"
     id: "418520"
     url: "https://proglib.io/p/frontend-whitelist/"
     date: "2017-03-12 13:05:12"
     humandate: "12 Mar, 2017"
     content: | 
       [&#8230;] Слепая доступность. Юрий Артюх [&#8230;]

     email: ""

  -  author: "Anthonyfen"
     id: "508676"
     url: "https://www.ninisilk.com/collections/silk-satin-pajamas"
     date: "2021-01-30 07:44:53"
     humandate: "30 Jan, 2021"
     content: | 
       <a href="https://www.ninisilk.com/collections/silk-satin-pajamas" rel="nofollow ugc">satin pajama set</a>
        
       Womens satin pajamas are each of the rage in the summer season months. Through the winter months, however, satin isn't a well-liked wardrobe staple. But this period, it can be switching everything. Women of all ages who love to lounge from the evening can now Activity satin pajamas having an update really feel and style.
       
       For the timeless glance, try a pair of mens satin pajamas with a major brushed chenille thread, double-sided satin pajamas having an ombre print, or even a clean satin pajama with embroidery. Up-to-date trend's Adult men's satin pajamas are usually created from extremely-mild, stretchy poly-silk Together with the related glimpse and texture of pure silk. Showcasing a secure elastic waistband, one particular button fly, and a entrance flap pocket within the chest, mens satin pajamas also can be found in huge, further massive, and medium measurements. They can be very easy to look after with just a wash in very hot drinking water and a mild detergent, and will last quite a long time. Most Adult males's satin sleepwear sets consist of pajama bottoms and slipcovers to safeguard them also.
       
       A person great way to retain expenditures down is to get an entire satin pajama established. Even so, for people who want to invest in just one piece, there are plenty of alternatives, such as a zip entrance zip up one-piece pajama established, a crew neck a person-piece set, or a strong coloration with satin or charmeuse overlays. Together with Value, quality and healthy also are essential factors when buying any sort of intimate clothing.
       
       The leading detail to contemplate when getting satin pajamas is flammability requirements. Most sleepwear brands foundation their flammability ratings on the level of heat produced through a dry warmth exam. Your best option for satin pajamas is robes that meet up with these minimal flammability requirements. Even if you do not plan to make use of the robe in open flames, It is really nevertheless a good idea to invest in robes which are rated for these reduced temperatures. Just in the event your satin pajamas catch fireplace within a fireplace, the upper ranking will make certain that it won't distribute greatly flames.
       
       There are various components that will have an impact on the expense of satin pajamas. By natural means, the fabric must be good quality and sturdy. Certain components are dearer than others, Primarily given that polyester is so extensively Utilized in satin fabric. Designer satin pajamas also are typically costlier. For a more economical solution, have a look at lower price sleepwear models for instance Valisere.
       
       Eventually, consider some great benefits of the satin pajamas set. If you need to continue to keep warm on cold evenings, then a two-piece satin pajama set might be The obvious way to go. Having said that, if you want paying time in incredibly hot shower rooms or soaking up the Sunshine while in the sun room, then a one particular-piece satin pajama set is probably finest. No matter whether you decide on sound hues or designs, be sure you buy satin sleepwear from the trustworthy company that meets flammability benchmarks.

     email: "talisman.slavik@mail.ru"

layout: "layouts/post.njk"
excerpt: "Познакомился с парнем который не видит, но делает сайты."
---

Познакомился с парнем который не видит, но делает сайты.<!--more-->
<h3>Мастеркласс Blind Accessibility от Дмитрия Попова</h3>
Вчера побывал на <a href="http://www.frontend-science.com/lab/">мастер-классе незрячего <strong>разработчика</strong></a> Дмитрия Попова, он выступал на последнем <a href="https://wsd.events/2016/11/26/">киевском WSD</a>, и ребята из Frontend-Science организовали отдельный развернутый воркшоп. И это было круто, немного информации, много ответов на вопросы, много реального опыта восприятия сайтов по-другому.


<h3>Что там было</h3>
Во-первых Дмитрий крутой перец. 

<h3>Удивительное для лично меня</h3>
Совершенно и искренне перевернуло мой мир веб-разработчика когда Дмитрий Попов в Devtools браузера исправил HTML сайта, для того чтобы он стал более доступным для скринридера. 

Подумайте об этом.

И еще немного.

Забавно, что Devtools браузера были свернуты так, что на экране их даже не было видно. Но все получилось. Потому что их и не надо было видеть. Ну да. 
О том что Дмитрий абсолютно без проблем отредактировал html страничку в notepad, наверное даже лишне говорить. Но его родной редактор в котором он пишет код: Nodepad++, как он сказал.

<p class="img"><img width="500" src="/images/a.jpg" alt=""><span>Тестируем разные сайты на доступность, под рукой у Дмитрия его "шпаргалки" набранные шрифтом Брайля</span></p>

Во-вторых поделюсь самыми главными мыслями, которые, надеюсь, помогут вам делать более доступные сайты.
<h3>Основное</h3>
<ul>
	<li>Вы никогда не узнаете кто использует ваш сайт.</li>
	<li>Сделать сайт доступным, несложно, обычно они почти все доступны из коробки. Но досадные ошибки разработчиков в мелочах, или их легкомысленность могут легко сделать сервис недоступным для других людей.</li>
	<li>Чтобы сделать сайт доступным обычно не нужно ничего переделывать. Лишь добавить немного смысла в код.</li>
	<li>Атрибут lang значит много, и если неверно задан доставляет много неудобств. Лучше не задавать никакой, чем неверный.</li>
</ul>

И несколько более конкретных примеров.
<h3>Кнопки-активные элементы</h3>
<strong>90% проблем</strong> при доступности сайтов возникает из-за того что активные элементы сделаны не кнопкой и не ссылкой. Если кнопка сделана как <code>&lt;div&gt;</code> то читалка не воспринимает его как активный элемент, и не помещает фокус на него при проходе страницы.

Чтобы решить эту проблему &#8212; просто используйте <code>&lt;button&gt;</code> или ссылку.

На худой конец используйте aria-label и <a href='https://www.w3.org/TR/wai-aria/roles'>role</a> (<code>role="button"</code>, например). Тогда читалка поставит фокус на этот элемент, и подскажет что он активный.

Например такая проблема есть на сайте Zakaz.ua
<p class="img"><img width="500" src="/images/a3.png" alt=""><span>Кнопка сделана ссылкой без href, и читалка не воспринимает ее как управляющий элемент</span></p>

<h3>Навигация по заголовкам</h3>
Оказывается очень удобно ходить по странице используя ее заголовки. На большинстве сайтов с этим все отлично, но на удивление на livejournal, заголовок статьи не является h1-h6 и тяжело найти начало текста. Вот например <a href="http://masterok.livejournal.com/3309231.html">подобная тема в живом журнале</a>
<h3>Отсылка к цветовой информации</h3>
Речь о всяких "Зеленые места свободны", это, причем распространяется не только на тех кто не видит, но и на тех кто видит цвета по-другому, а таких людей очень немало. Стоит дублировать эту информацию альтернативным способом.

Например, Яндекс Карты, показывая пробки, дублируют информацию о пробке(это красная заливка) плотностью стрелочек на дороге. Я и не задумывался зачем это, пока Сергей Пузанков не рассказал.
<p class="img"><img width="500" src="/images/a1.png" alt=""><span>Обратите внимание на длину стрелочек там где пробка и где её нет</span></p>

<h3>Атрибут lang</h3>
Когда он задан неверно, читалка пытается читать русский текст с английской транскрипцией, и на скорости 400 слов в минуту это ужасно и вообще непонятно. Дмитрий рекомендовал задавать его даже для частей страницы, чтобы читалки экрана правильно произносили слова.

<h3>Не забывать об этом</h3>
Это конечно не полный список, но все это несложно, нужно просто не забывать о том что вашим сайтом будут пользоваться совершенно разные люди. И прекрасно, что и поисковая оптимизация, и семантика кода, и многое другое на самом деле косвенно помогает нам делать сайты более доступными для всех.

<ul>
	<li><a href="https://www.w3.org/WAI/intro/aria">Главная страница о доступности в веб-стандартах</a></li>
	<li>Нашел случайно статью о том как работают <a href="https://habrahabr.ru/post/262363/">другие незрячие разработчики</a></li>
<li><a href="https://www.facebook.com/frontendscience/posts/2067329360160106">Пара фото с воркшопа</a></li>
<li><a href="http://gov.design/blog/2016/11/08/accessibility.html">Чеклист доступности сайта от разработчиков государственных сайтов в России</a></li>
</ul>
