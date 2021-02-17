---
title: "Cколько-то способов min-height"
date: "2007-11-29"
humanDate: "29 Nov, 2007"
permalink: "2007/11/29/min-height/"
tags: 
  - "xhtmlcss"
  - "useful"
comments: 
  -  author: "Sam"
     id: "11375"
     url: "http://rmcreative.ru/"
     date: "2007-11-29 18:20:38"
     humandate: "29 Nov, 2007"
     content: | 
       Давно пользуюсь №1. Про второй не знал. Expression не люблю.

     email: "sam@rmcreative.ru"

  -  author: "akella"
     id: "11376"
     url: "http://cssing.org.ua"
     date: "2007-11-29 18:28:41"
     humandate: "29 Nov, 2007"
     content: | 
       2 и 3й уже скорее дань истории, пока не было min-height в ИЕ7(а в бетах ее не было) приходилось к ним прибегать.

     email: "seijuro@yandex.ru"

  -  author: "romand"
     id: "11377"
     url: "http://uadrom.com/"
     date: "2007-11-29 18:48:51"
     humandate: "29 Nov, 2007"
     content: | 
       якщо мета питання про min-height - приліпити .footer до нижньої межі "бровзера" - 
       http://www.themaninblue.com/experiment/footerStickAlt/

     email: "roman.dorosh@gmail.com"

  -  author: "Zigzag"
     id: "11378"
     url: "http://webdev.lovata.com"
     date: "2007-11-29 19:19:21"
     humandate: "29 Nov, 2007"
     content: | 
       молодца, давно было их все вместе собрать =)

     email: "zigzag.mcquack@gmail.com"

  -  author: "akella"
     id: "11379"
     url: "http://cssing.org.ua"
     date: "2007-11-29 20:14:07"
     humandate: "29 Nov, 2007"
     content: | 
       romand: мета може бути різною - я частіше використовував для чисто дизайнерськіх моментів, але лінк звісно хороший та відомий - нехай буде =)
       
       Zigzag: дякую!

     email: "seijuro@yandex.ru"

  -  author: "Dimox"
     id: "11380"
     url: "http://dimox.name"
     date: "2007-11-29 22:30:00"
     humandate: "29 Nov, 2007"
     content: | 
       Первым способом пользуюсь постоянно. Про второй не знал. Спасибо за него.

     email: "dimox.name@mail.ru"

  -  author: "Slaver"
     id: "11381"
     url: "http://slaver.cutenews.ru"
     date: "2007-11-29 23:41:56"
     humandate: "29 Nov, 2007"
     content: | 
       Только первый вариант! :)

     email: "radionov@gmail.com"

  -  author: "Mourner"
     id: "11382"
     url: "http://agafonkin.com"
     date: "2007-11-30 01:58:56"
     humandate: "30 Nov, 2007"
     content: | 
       Экспрешнами по возможности лучше не пользоваться. Вредит сильно быстродействию (кроме того, что JS-зависимо).
       
       Второй способ требует дополнительного элемента в маркапе.
       
       Так что лично для меня только первый :)

     email: "agafonkin@gmail.com"

  -  author: "Руслан"
     id: "11383"
     url: ""
     date: "2007-11-30 10:48:05"
     humandate: "30 Nov, 2007"
     content: | 
       Если работает первый метод, то зачем изобретать велосипед?
       В любом случае, интересно было узнать что-то новое (2й и 3й метод =) Спасибо!

     email: "w3m@rambler.ru"

  -  author: "agat"
     id: "11384"
     url: "http://romanovskij.ru"
     date: "2007-11-30 10:52:20"
     humandate: "30 Nov, 2007"
     content: | 
       А Conditional Comments использовать для чистоты основного CSS-файла это уже не модно? :) И никаких странных хаков, перехаков.

     email: "aleksij@gmail.com"

  -  author: "akella"
     id: "11385"
     url: "http://cssing.org.ua"
     date: "2007-11-30 10:52:26"
     humandate: "30 Nov, 2007"
     content: | 
       дада, так и есть, просто я проморгал поддержку min-height у IE7, и пост этот писал чуть не год назад, когда это было актуально, просто вот подзадержался он =). Стоит убрать этот один маленький нюанс - и уже нужны все три метода. :) Вобщем то на данный момент самым простым и правильным остается первый. Эх как быстро время бежит
       
       @ЖенатыйAgat: дык хаки то валидные =) Чего лишний раз кондкомментить

     email: "seijuro@yandex.ru"

  -  author: "akira"
     id: "11386"
     url: "http://akira.spb.su"
     date: "2007-11-30 11:12:02"
     humandate: "30 Nov, 2007"
     content: | 
       Что-то я не понимаю про expression.
       Это все браузеры поймут?
       А какие преимущества перед JavaScript в отдельном файле?

     email: "akira@phpcom.ru"

  -  author: "akella"
     id: "11387"
     url: "http://cssing.org.ua"
     date: "2007-11-30 11:16:30"
     humandate: "30 Nov, 2007"
     content: | 
       Преимущества, что его(js) только ради этих целей можно не создавать, а описать это поведение в CSS. Оно отчасти и логично, ведь все что делает этот кусочек js &#8212; это эмуляция CSS свойства min-height.
       
       Поймет это конечно только IE, а все остальные уже поддерживают min-height.

     email: "seijuro@yandex.ru"

  -  author: "lusever"
     id: "11392"
     url: "http://lusever.livejournal.com/"
     date: "2007-11-30 13:21:51"
     humandate: "30 Nov, 2007"
     content: | 
       Я выложу :)
       
       height: expression(this.scrollHeight < 201px ? "200px" : "auto" );
       меняется на
       height: expression(scrollHeight < 201 ? "200px" : "auto" );
       
       Прооптимизировать это для динамического контента, или, если требуется зависимость от ширины окна браузера невозможно.
       
       Еще есть способ, задать минимальную ширину вставив прозрачный gif, например тем же экспрешеном, вот это запросто оптимизируется. Можно развернуться и красиво написать.

     email: "ufokorpas@mail.ru"

  -  author: "rr"
     id: "11400"
     url: ""
     date: "2007-11-30 21:03:52"
     humandate: "30 Nov, 2007"
     content: | 
       а как на счет
       <pre>.block {
        min-height:200px;
        *height:200px;
       }</pre>
       или валидность на первом месте?)

     email: "rr-m@tut.by"

  -  author: "akella"
     id: "11401"
     url: "http://cssing.org.ua"
     date: "2007-11-30 21:08:05"
     humandate: "30 Nov, 2007"
     content: | 
       Отличный рабочий вариант, но тот(Дастина Диаза) не так из-за валидности рулит, как из-за future-proof.
       Кто их знает как броузеры будут понимать эту * через пару лет, а !important - все же четко описан. Да и сафари иногда грешит пониманием невалидных ЦСС.
       
       Впрочем де факто думаю это решение еще года два можно смело применять. =) не забывая тестить

     email: "seijuro@yandex.ru"

  -  author: "Sukebe"
     id: "11403"
     url: "http://sukebe.ru"
     date: "2007-12-01 21:02:37"
     humandate: "01 Dec, 2007"
     content: | 
       Мой вариант такой:
       <pre>.block {
        min-height: 200px;
       }
       * html .block {
        height: 200px;
       }</pre>

     email: "dm@sukebe.ru"

  -  author: "Shimon"
     id: "11406"
     url: "http://www.chossonandkallah.com"
     date: "2007-12-03 07:14:33"
     humandate: "03 Dec, 2007"
     content: | 
       Спасибо, пригодится!
       Вот только у меня тот же вопрос возник, что и у Романа выше - зачем нужны другие способы если есть первый?

     email: "shimonenator@gmail.com"

  -  author: "akella"
     id: "11407"
     url: "http://cssing.org.ua"
     date: "2007-12-03 11:17:09"
     humandate: "03 Dec, 2007"
     content: | 
       Я в 11 комментарии вроде как ответил =) Теперь уже больше для справки и как примеры идей, которые возможно применить в других областях.
       
       К примеру второй метод можно легко приложить к кендо.

     email: "seijuro@yandex.ru"

  -  author: "gordi"
     id: "11408"
     url: "http://trifler.ru/blog/"
     date: "2007-12-03 14:54:03"
     humandate: "03 Dec, 2007"
     content: | 
       По второму способу заморачивался не давно:
       http://trifler.ru/blog/post_1192811790.html
       http://trifler.ru/blog/post_1193561490.html
       Увы, масса дополнительных блоков является большим минусом.
       Поэтому варианты 1 и 3 предпочтительней.

     email: "serg-girdi@mail.ru"

  -  author: "Tutta Karlsson"
     id: "11425"
     url: ""
     date: "2007-12-07 15:40:02"
     humandate: "07 Dec, 2007"
     content: | 
       Все изложенные способы не очень практичны и ущербны.
       1. Для эластичной верстки, как правило, часто блоку необходимо ДЕРЖАТЬ ВЫСОТУ ОКНА и только в случае малых размеров скролироваться, сохраняя дизайн и целостность юзабилити. При этом фиксированная в 200px высота не катит и след. метод №1 тоже не катит. 
       Остается скрипт все равно в виде expression или js.
       width: expression(document.body.clientHeight &gt; 200 ? "100%" : "200px")
       
       2. НО Действительно НАСТОЯЩЕЙ проблемой на сегодняшний момент является проблема больших мониторов (24" и более), которых становится уже предостаточно. Проблема состоит в том - каким образом установить ОДНОВРЕМЕННО min-height и max-height ????

     email: "springer@mail.ru"

  -  author: "akella"
     id: "11426"
     url: "http://cssing.org.ua"
     date: "2007-12-07 15:55:50"
     humandate: "07 Dec, 2007"
     content: | 
       1) Вы видимо имели ввиду резиновой верстки? Эластичная &#8212; это зависимая от размера шрифта, такая принята терминология. 
       Решение проблемы высоты в экран куда проще - http://www.themaninblue.com/experiment/footerStickAlt/. Если я неправильно понял - покажите сайт с тем поведением которого вы хотите достигнуть, а то я слегка запутался в том почему методы не катят.
       
       
       2) А что в этом такого? Так же как и min-max width http://uggallery.audiopeace.ru/2007/10/27/min-max-width-ie5-6 замените width на height и все. Чем такой вариант Вам неподошёл?
       Или вот еще более оптимизированный - http://www.gunlaug.no/contents/wd_additions_14.html
       <pre>CSS for standard compliant browsers:
       
       #wrapper {width: 99%;
       max-width: 1200px; 
       min-width: 550px;}
       
       CSS for MSIE/win:
       
       * html div#wrapper {width: 760px /* fallback value */;
       width:expression(((document.compatMode && 
       document.compatMode=='CSS1Compat') ? 
       document.documentElement.clientWidth : 
       document.body.clientWidth) 
       > 1218 ? '1200px' : (((document.compatMode && 
       document.compatMode=='CSS1Compat') ? 
       document.documentElement.clientWidth : 
       document.body.clientWidth) < 570 ? '552px' : '99.7%')); }
       </pre>
       
       А <a href="http://gnillydev.blogspot.com/2007/10/min-width-min-height-max-width-max.html">Тут</a> вообще специальный джаваскрипт для таких целей написали =)

     email: "seijuro@yandex.ru"

  -  author: "Serge"
     id: "11493"
     url: ""
     date: "2007-12-18 16:14:39"
     humandate: "18 Dec, 2007"
     content: | 
       2 Sukebe +1
       
       правильный ответ 1 !!!!

     email: "bob_s@list.ru"

  -  author: "Андрей"
     id: "11598"
     url: "http://www.univer.by"
     date: "2008-01-06 01:49:43"
     humandate: "06 Jan, 2008"
     content: | 
       Отличный сайт, отличный контент. В работе ваши рекомендации помогут.

     email: "student@univer.by"

  -  author: "Jen"
     id: "14320"
     url: "http://www.svarga.biz"
     date: "2009-04-01 11:17:20"
     humandate: "01 Apr, 2009"
     content: | 
       может, я что-то не так делаю, но по первому способу это работает, только до какой-то высоты (около 20 пикселов). Сделать min-height 1px это не помогло.

     email: "sneer@hitv.ru"

  -  author: "Обзор №3, Январь 2008 - Design For Masters"
     id: "13267"
     url: "http://designformasters.info/posts/review-january-2008/"
     date: "2008-09-21 02:28:43"
     humandate: "21 Sep, 2008"
     content: | 
       [...] Cколько-то способов min-height Min-height свойство нужное, часто полезное, но&nbsp;в&nbsp;Internet Explorer не&nbsp;работает, вразумить его можно несколькими способами о&nbsp;которых и&nbsp;идет речь. [...]

     email: ""

  -  author: "Сергей"
     id: "18637"
     url: ""
     date: "2010-04-30 19:28:54"
     humandate: "30 Apr, 2010"
     content: | 
       Пример где min-height имитируется с помощью important не работает в ie8 (где так же не работают min-height). Если для div указать overflow:hidden то ie будет обрезать данные, а ff и opera будут отображать нормально

     email: "n3n@mail.ru"

layout: "layouts/post.njk"
excerpt: "Несколько способов реализации min-height для всех броузеров. Короткий обобщающий пост. Надеюсь все оценили как я изящно избежал цифры в названии поста?=)
"
---

Несколько способов реализации min-height для всех броузеров. Короткий обобщающий пост. Надеюсь все оценили как я изящно избежал цифры в названии поста?=)
<!--more-->
Свойство нужное, часто полезное, но в Internet Explorer не работает. Далее способы вразумить синюю букву Е.

<h3>1. min-height через height</h3>
Говорят, разработчики IE5-6 <strong>реализовали</strong> свойство min-height, просто решили его назвать height, так оно вобщем то и есть. height для 5й и 6й версий ведет себя как min-height. В 7й версии min-height уже работает. Потому вопрос лишь в том, как им всем отдать свои значения. Об этом позаботился Дастин Диаз:
<ol class="code">
<li>.block {</li>
<li class="tab">min-height:200px;</li>
<li class="tab">height:auto !important;</li>
<li class="tab">height:200px;</li>
<li>}</li></ol>
Комментировать особо нечего - это работает. Первая колонка в <a href="http://cssing.org.ua/examples/min-height/">примере</a>.

На данный момент, в силу того что ИЕ7 уже поддерживает min-height, два другие способа я привожу скорее как историческую справку и пример интересных приемов.
<ul>
<li><a href="http://www.dustindiaz.com/min-height-fast-hack/">оригинальная статья</a></li>
</ul>
<h3>2. min-height с помощью padding</h3>
Так же можно эмулировать минимальную высоту с помощью комбинации:
<ol class="code">
<li>.block{padding-top:200px}</li>
<li>.block .inner{margin-top:-200px}</li>
</ol>
Этот способ требует однако дополнительного элемента ".inner", тем не менее является пожалуй самым простым и иногда удобным.
Что бы кусок кода был максимально универсальным - лучше добавлять аж 2 обертки:
<ol class="code">
<li>.block .inner{padding-top:200px}</li>
<li class="tab">.block .inner1{margin-top:-200px}</li>
</ol>
В <a href="http://cssing.org.ua/examples/min-height/">примере</a> я вместо второй обертки использовал элемент h2.
<ul>
<li>Подробнее в блоге <a href="http://www.mezzoblue.com/archives/2004/09/16/minheight_fi/">у Dave Shea</a></li>
</ul>
<h3>3. min-height с помощью expression</h3>
Как всегда все можно решить с помощью джаваскрипт.

До того как вышла 7ая версия можно было делать так:
<ol class="code">
<li>.block{height: expression('32px'); min-height: 32px;}</li>
</ol>
Однако этот вариант не работает в 7й версии.

Более универсально и в лоб, проблема решается так:
<ol class="code">
<li>.block { </li>
<li class="tab">height: expression(this.scrollHeight < 201px ? "200px" : "auto" ); </li>
<li class="tab">min-height: 200px; </li>
<li>}</li>
</ol>
Или что бы ускорить работу скрипта, как <a href="http://cssing.org.ua/2007/11/29/min-height/#comment-11392">советует</a> <a href="http://lusever.ru">Павел Корнилов</a>, <code>this</code> можно опустить:
<ol class="code">
<li>.block { </li>
<li class="tab">height: expression(scrollHeight < 201px ? "200px" : "auto" ); </li>
</ol>
Для body, однако, так нельзя оптимизировать.
<h3>В конце</h3>
<ul>
<li><a href="http://cssing.org.ua/examples/min-height/">Пример с тремя методами</a></li>
</ul>
Буду рад услышать ваши методы и мысли по поводу решения этой проблемы!
