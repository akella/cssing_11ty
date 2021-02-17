---
title: "overflow:hidden"
date: "2010-04-26"
humanDate: "26 Apr, 2010"
permalink: "2010/04/26/overflow-hidden/"
tags: 
  - "xhtmlcss"
comments: 
  -  author: "Юрко"
     id: "18590"
     url: ""
     date: "2010-04-26 11:26:13"
     humandate: "26 Apr, 2010"
     content: | 
       Свєжак!

     email: "aaa@zzz.xxx"

  -  author: "miripiruni"
     id: "18591"
     url: "http://miripiruni.org"
     date: "2010-04-26 11:30:03"
     humandate: "26 Apr, 2010"
     content: | 
       Почему же? Очень даже популярный прием, среди меня, например ;)
       
       Кстати у Flack'а есть <a href="http://flack.ru/2008/08/26/semantic-coding-howto-6/" rel="nofollow">старенький пост</a> пhо это же поведение.

     email: "miripiruni@gmail.com"

  -  author: "akella"
     id: "18592"
     url: "http://cssing.org.ua"
     date: "2010-04-26 11:34:03"
     humandate: "26 Apr, 2010"
     content: | 
       Значит он просто проходил мимо меня, я ж и не говорю что новый, но пара знакомых точно не знала :) А тут я наконец нашел причину, и она весьма законная и решил привлечь внимание ;)

     email: "akella.a@gmail.com"

  -  author: "macgera"
     id: "18589"
     url: "http://macgera.com.ua"
     date: "2010-04-26 11:22:38"
     humandate: "26 Apr, 2010"
     content: | 
       Блог Tips&amp;Tricks по CSS))) или вообще How to ))))

     email: "macgera@gmail.com"

  -  author: "Антон Вернигор"
     id: "18597"
     url: ""
     date: "2010-04-26 11:57:07"
     humandate: "26 Apr, 2010"
     content: | 
       Немного спокойнее использовать для этого overflow: auto, при этом достигается тот же эффект.

     email: "smmurf@yandex.ru"

  -  author: "akella"
     id: "18598"
     url: "http://cssing.org.ua"
     date: "2010-04-26 12:01:07"
     humandate: "26 Apr, 2010"
     content: | 
       Да, но к сожалению на практике он иногда вызывает появление скроллинга =(

     email: "akella.a@gmail.com"

  -  author: "Genn"
     id: "18593"
     url: "http://genn.org/"
     date: "2010-04-26 11:40:09"
     humandate: "26 Apr, 2010"
     content: | 
       CSS4 as is!

     email: "soap@genn.org"

  -  author: "ask"
     id: "18604"
     url: ""
     date: "2010-04-26 16:13:39"
     humandate: "26 Apr, 2010"
     content: | 
       После мастер-класса только так и делаю для блоков фикс+резина ;) Действительно, очень просто, удобно и работает везде, где требуется.

     email: "ask.dev@gmail.com"

  -  author: "Николай"
     id: "18605"
     url: ""
     date: "2010-04-26 16:19:49"
     humandate: "26 Apr, 2010"
     content: | 
       А еще если кто-то вдруг вздумает оформлять таким способом иконки или другие мелкие картинки, помните о том что в FF текст обрезается на 1px по краям и нужно делать padding:1px; для блока с overflow:hidden; Кстати, при редизайне сайта <a href="http://www.w3.org/" rel="nofollow">W3C</a> активно использовался этот метод.

     email: "gruzzilkin@gmail.com"

  -  author: "Глеб Арестов"
     id: "18608"
     url: "http://arestov.me"
     date: "2010-04-26 17:31:21"
     humandate: "26 Apr, 2010"
     content: | 
       Кому интересна данная тема предлагаю ознакомится ещё вот с этими статейками :)
       
       Clear или overflow:hidden — очистка всего потока или создание контекста форматирования?
       http://habrahabr.ru/blogs/css/48383/
       
       Управление потоком в CSS: создаём контекст форматирования
       http://habrahabr.ru/blogs/css/48429/

     email: "gr1b0k@gmail.com"

  -  author: "GreLI"
     id: "18595"
     url: ""
     date: "2010-04-26 11:45:53"
     humandate: "26 Apr, 2010"
     content: | 
       Ну вообще-то всё это можно было узнать, прочитав первый абзац из <a href="http://www.w3.org/TR/CSS2/visuren.html#block-formatting" rel="nofollow">Block formatting contexts</a>: «Floats, absolutely positioned elements, inline-blocks, table-cells, table-captions, and elements with <b>'overflow' other than 'visible'</b> (except when that value has been propagated to the viewport) establish new block formatting contexts.» (выделение моё) и далее.
       
       С overflow:hidden есть такая проблема, что обрезается всё что вылезает за пределы. Например, можно сделать резиновый инпут с кнопкой, но подсказку (например, список вариантов строк поиска) к нему уже не отобразишь: обрежется. Только если извращаться так, чтобы позиционирование было относительно блока вне этого overflow, хоть позиционировать хочется и относительно содержимого.

     email: "greli@mail.ru"

  -  author: "akella"
     id: "18596"
     url: "http://cssing.org.ua"
     date: "2010-04-26 11:49:45"
     humandate: "26 Apr, 2010"
     content: | 
       @GreLI Благодарю! Но я ж именно для этого я и вставил эту же цитату в пост. А правда в том что 99% не читают спецификацию. Я, например. ;) А когда не подходит overflow всегда можно вернуться к старому доброму display:table и поизвращаться по-другому.

     email: "akella.a@gmail.com"

  -  author: "Genn"
     id: "18599"
     url: "http://genn.org/"
     date: "2010-04-26 12:02:03"
     humandate: "26 Apr, 2010"
     content: | 
       akella и GreLl, самое крутое, что спецификацию не читают создатели браузеров! ;)

     email: "soap@genn.org"

  -  author: "mktums"
     id: "18600"
     url: "http://miketums.net"
     date: "2010-04-26 12:16:19"
     humandate: "26 Apr, 2010"
     content: | 
       Вот! Вот чего не хватает!
       Приемы, хаки, how-to!
       
       Спасибо за статью :)

     email: "mktums@gmail.com"

  -  author: "GreLI"
     id: "18601"
     url: ""
     date: "2010-04-26 12:55:43"
     humandate: "26 Apr, 2010"
     content: | 
       Genn, читать-то читают, но там свои заморочки. Текст в спецификации мог сильно меняться со временем. Лет 10 назад эти моменты были гораздо менее ясны.

     email: "greli@mail.ru"

  -  author: "private_face"
     id: "18609"
     url: ""
     date: "2010-04-26 18:39:42"
     humandate: "26 Apr, 2010"
     content: | 
       В своем примере (http://cssing.org.ua/examples/overflow-hidden/index_layout.html) вы забыли установить hasLayout для колонки .center. Если контента в центральной части будет больше, чем в колонках, этот контент начнет колонки обтекать.
       
       Если же hasLayout установить, то в IE6 между float колонками и центральной частью появляется 3px отступ. Можно, конечно, пофиксить отрицательными маргинами, но как-то некрасиво. Может есть способ попроще?

     email: "private.face@gmail.com"

  -  author: "Олег"
     id: "18610"
     url: ""
     date: "2010-04-26 23:04:46"
     humandate: "26 Apr, 2010"
     content: | 
       Мы всё-таки используем clearfix, потому что в современных сайтах очень много всяких выпадушек и прочих прыгающих элементов и проще навесить какой-нибудь глобальный класс (типа .clearfix), который исправляет эту проблему, нежели мучаться с overflow.

     email: "oleg.mokhov@gmail.com"

  -  author: "Maksim"
     id: "18611"
     url: ""
     date: "2010-04-27 00:08:17"
     humandate: "27 Apr, 2010"
     content: | 
       Ну раз уж речь пошла об "overflow: hidden", то я тогда не удержусь про "быстрый clearfix" без всяких :after.
       Если родителю задать свойство "overflow: hidden", то он так же не дает выпрыгивать из себя внутренние блоки с обтеканием как.
       Тем же самым свойством обладают, табличные и inline-block элементы.
       
       Конечно не америку открыл, но мало ли кому-то будет полезным.

     email: "biserov.ma@gmail.com"

  -  author: "Никита Селецкий"
     id: "18612"
     url: "http://seleckis.lv"
     date: "2010-04-27 00:45:22"
     humandate: "27 Apr, 2010"
     content: | 
       Олег и Maksim, по-моему тут речь идёт не о clearfix. Если бы это был контейнер с плавающим блоком внутри, то да. А здесь плавающий блок, а за ним идёт блок в общем потоке, который игнорирует плавающий, а внутренние строковые элементы обтекают «поплавок».
       
       akella, а чем это лучше margin: «ширина зафлоаченного блока»? Разве что на строчку меньше писать, но зато больше контроля, мне кажется.

     email: "nikita@seleckis.lv"

  -  author: "Никита Селецкий"
     id: "18613"
     url: "http://seleckis.lv"
     date: "2010-04-27 00:46:21"
     humandate: "27 Apr, 2010"
     content: | 
       имеется в виду margin-left или margin-right в зависимости от того, где блоки находятся.

     email: "nikita@seleckis.lv"

  -  author: "Олег"
     id: "18614"
     url: ""
     date: "2010-04-27 00:53:33"
     humandate: "27 Apr, 2010"
     content: | 
       Никита, вы правы, Юра прошу прощения.
       
       Соответственно я отвечу на ваш вопрос про margin: в данном случае мы получаем возможность не зависеть от ширины обтекаюемого блока.
       
       Юра, всё-таки несмотря на это мне кажется overflow:hidden хуже display: table именно по причине опять же невозможности выносить из него абсолютно позиционированные элементы. Хотя надо поэкспериментировать, вроде как в норм.браузерах все должно быть ок, а для ие zoom: 1 + position: relative.

     email: "oleg.mokhov@gmail.com"

  -  author: "GreLI"
     id: "18617"
     url: ""
     date: "2010-04-27 08:35:27"
     humandate: "27 Apr, 2010"
     content: | 
       Никита Селецкий, это лучше тем, что ширина флоата может быть совершенно неизвестной и менятся в зависимости условий. Например, в случае с инпутом и кнопкой, на кнопке текст может оказать написанный неизвестным шрифтом и размером, а сам он может различен в зависимости от языка.

     email: "greli@mail.ru"

  -  author: "Никита Селецкий"
     id: "18618"
     url: "http://seleckis.lv"
     date: "2010-04-27 13:43:03"
     humandate: "27 Apr, 2010"
     content: | 
       Спасибо за разъяснение.

     email: "nikita@seleckis.lv"

  -  author: "Никита Селецкий"
     id: "18626"
     url: "http://seleckis.lv"
     date: "2010-04-29 14:23:00"
     humandate: "29 Apr, 2010"
     content: | 
       private_face, 3 пиксельный отступ лучше фиксировать отрицательным маргином именно у плавающей картинки.

     email: "nikita@seleckis.lv"

  -  author: "akella"
     id: "18624"
     url: "http://cssing.org.ua"
     date: "2010-04-28 17:33:46"
     humandate: "28 Apr, 2010"
     content: | 
       Спасибо Глеб! Добавил обе ссылки в пост! (Там только картинки покорежились жаль=()
       
       @private_face Да, действительно, увлекся отказом от IE6 ;)

     email: "akella.a@gmail.com"

  -  author: "float &#8211; запрет обтекания с помощью overflow:hidden &laquo; Artycreate 4developers blog"
     id: "18631"
     url: "http://4dev.artycreate.net/2010/04/30/float-%d0%b7%d0%b0%d0%bf%d1%80%d0%b5%d1%82-%d0%be%d0%b1%d1%82%d0%b5%d0%ba%d0%b0%d0%bd%d0%b8%d1%8f-%d1%81-%d0%bf%d0%be%d0%bc%d0%be%d1%89%d1%8c%d1%8e-overflowhidden"
     date: "2010-04-30 11:23:40"
     humandate: "30 Apr, 2010"
     content: | 
       [...] Сама статья: http://cssing.org.ua/2010/04/26/overflow-hidden/ [...]

     email: ""

  -  author: "Jman"
     id: "18658"
     url: "http://myopinion.net.ua"
     date: "2010-05-17 15:58:35"
     humandate: "17 May, 2010"
     content: | 
       я с самого начала использовал повсеместно overflow:hidden; zoom:1; так как считал table-cell а тем более :after{clear:both} лишними финтами.

     email: "jman.ua@gmail.com"

  -  author: "Eduard"
     id: "18650"
     url: "http://profitgid.ru/"
     date: "2010-05-07 15:57:21"
     humandate: "07 May, 2010"
     content: | 
       Так намного лучше! Мне понравилось, буду пользоваться!

     email: "polbeduard@mail.ru"

  -  author: "Del'ka"
     id: "18645"
     url: "http://delka.name"
     date: "2010-05-05 10:35:35"
     humandate: "05 May, 2010"
     content: | 
       Клёво! Реально клёво!
       
       Спеку читать тяжко, я смог осилить лишь спеку по html4 и то заставлял себя читать каждый день хоть по несколько экранов с мобилки по дороге домой. А у Мейера в книге про такой интересный финт не рассказывалось.

     email: "delka@anime.kharkov.ua"

  -  author: "warmrobot"
     id: "18681"
     url: "http://igorfrolov.info"
     date: "2010-05-28 15:32:08"
     humandate: "28 May, 2010"
     content: | 
       И да придёт спаситель! )) Только что столкнулся с тем, что контент переносился со строчки на строчку, так как его сжимал объемлющий display: table. Спасибо!

     email: "igorfrolov@igorfrolov.info"

  -  author: "Парад статей для css и html разработчиков | Masterix.com.ua | Блог для тех кто верстает."
     id: "18688"
     url: "http://masterix.com.ua/2010/06/parad-statej-dlya-css-i-html-razrabotchikov/"
     date: "2010-06-01 13:52:07"
     humandate: "01 Jun, 2010"
     content: | 
       [...] Overflow:hidden от отлиного сайта cssing.org.ua. Отличное решение проблемы обтекания картинки текстом. Можно так же вспомнить как это делалось раньше и что предлагает сделать автор сейчас. [...]

     email: ""

  -  author: "evgeni"
     id: "18713"
     url: "http://inmybook.ru/evgeni"
     date: "2010-06-21 19:35:18"
     humandate: "21 Jun, 2010"
     content: | 
       Интересное решение. Вы откуда их берете, из своего опыта или из документации?

     email: "inmybook@yandex.ru"

  -  author: "Lemberg"
     id: "18739"
     url: "http://postcards.org.ua/"
     date: "2010-07-12 09:58:21"
     humandate: "12 Jul, 2010"
     content: | 
       Достойный прочтения материал, раньше даже не задумывался о возможных способах решения, как правило, лепил наспех таб с двумя колонками. Будем использовать, пасиб)

     email: "pc-lemberg@yandex.ru"

  -  author: "Levik"
     id: "18776"
     url: "http://www.levik.info"
     date: "2010-08-19 16:49:23"
     humandate: "19 Aug, 2010"
     content: | 
       Есть ещё один, ещё более "старенький" пост в котором упоминается о поведении overflow:hidden... 
       http://cssing.org.ua/2005/11/24/css-simple-two-columns/

     email: "ivan-lev@mail.ru"

  -  author: "maxim"
     id: "18832"
     url: "http://kinomooviz.ru"
     date: "2010-09-22 09:50:34"
     humandate: "22 Sep, 2010"
     content: | 
       попробую сегодня у себя

     email: "maximfro@mail.ru"

  -  author: "Индивидуалки"
     id: "18814"
     url: "http://inprostitute-kiev.com"
     date: "2010-09-14 12:48:43"
     humandate: "14 Sep, 2010"
     content: | 
       интересная статья

     email: "inpro@mail.ru"

  -  author: "igor"
     id: "18815"
     url: "http://golden-comp.ru"
     date: "2010-09-15 10:57:48"
     humandate: "15 Sep, 2010"
     content: | 
       отличная статья.

     email: "igorzeinalov@mail.ru"

  -  author: "evgenii"
     id: "18816"
     url: "http://bakemono.ru/"
     date: "2010-09-16 10:42:19"
     humandate: "16 Sep, 2010"
     content: | 
       О, отличный способ, спасибо)

     email: "evgeniidrobonyuk@mail.ru"

  -  author: "vanchelo"
     id: "18855"
     url: ""
     date: "2010-09-23 16:47:39"
     humandate: "23 Sep, 2010"
     content: | 
       А margin-left - почему нельзя использовать

     email: "vanchelo@lavabit.com"

  -  author: "akella"
     id: "18857"
     url: "http://cssing.org.ua"
     date: "2010-09-23 17:01:20"
     humandate: "23 Sep, 2010"
     content: | 
       Потому что для margin-left нужно знать ширину картинки, а с overflow:hidden делается универсально.

     email: "akella.a@gmail.com"

  -  author: "vanchelo"
     id: "18860"
     url: ""
     date: "2010-09-23 18:39:23"
     humandate: "23 Sep, 2010"
     content: | 
       В этом плане, я согласен

     email: "vanchelo@lavabit.com"

  -  author: "css свойство float &#8211; запрет обтекания с помощью overflow:hidden | DVA home page"
     id: "18869"
     url: "http://dva.sumy.ua/2010/04/30/css-%d1%81%d0%b2%d0%be%d0%b9%d1%81%d1%82%d0%b2%d0%be-float-%d0%b7%d0%b0%d0%bf%d1%80%d0%b5%d1%82-%d0%be%d0%b1%d1%82%d0%b5%d0%ba%d0%b0%d0%bd%d0%b8%d1%8f-%d1%81-%d0%bf%d0%be"
     date: "2010-09-24 14:40:50"
     humandate: "24 Sep, 2010"
     content: | 
       [...] статья: http://cssing.org.ua/2010/04/26/overflow-hidden/ This entry was posted in Posts and tagged css. Bookmark the permalink. Инструкция [...]

     email: ""

  -  author: "kvex"
     id: "18931"
     url: ""
     date: "2010-11-04 13:06:01"
     humandate: "04 Nov, 2010"
     content: | 
       Использую для очитски действия float:
       overflow: hidden; - для нормальных браузеров
       width: 100%; (или в пикселях) - для IE

     email: "vasiliy.v.nesterenko@gmail.com"

  -  author: "Очередной вебмастер"
     id: "21535"
     url: "http://k2joomla.ru"
     date: "2011-09-10 15:25:45"
     humandate: "10 Sep, 2011"
     content: | 
       Вы мой спаситель, сам начинающий верстальщик, и это вопрос мне не дает покоя уже полгода, чтоб картинка была слева, а текст справа обтекал, но при этом не был под ней )))
       Все гениальное просто. Еще раз спасибо.

     email: "bizezine@gmail.com"

  -  author: "Вебмастер"
     id: "24548"
     url: "http://doramakun.ru/"
     date: "2011-10-28 14:32:56"
     humandate: "28 Oct, 2011"
     content: | 
       Да, но согласитесь, верстать нынче стало проще!

     email: "johny@dtaft.ru"

layout: "layouts/post.njk"
excerpt: "Незаслуженно непопулярный трюк. Я уже писал про <a href=\"http://cssing.org.ua/2005/07/03/display-table/\">display:table</a>. Так вот, это &#8212 лучше. P.S.: оказалось трюк таки известен многим, надеюсь кому-то статья поможет."
---

Незаслуженно непопулярный трюк. Я уже писал про <a href="http://cssing.org.ua/2005/07/03/display-table/">display:table</a>. Так вот, это &#8212 лучше. P.S.: оказалось трюк таки известен многим, надеюсь кому-то статья поможет.<!--more-->
<h3>Проблема</h3>
Еще пять лет назад я искал решение проблемы: как запретить обтекание float. Подробнее можно читать в <a href="http://cssing.org.ua/2005/07/03/display-table/">старом посте</a> (2005 год, офигеть). Вкратце, мы приводили это:
<p class="img con"><img src="http://cssing.org.ua/pic/overflow/1.png" width="377" height="133" /><span>Картинка-float</span></p>
к такому виду:
<p class="img con"><img src="http://cssing.org.ua/pic/overflow/2.png" width="377" height="149" /><span>Картинка-float + display:table для текста</span></p>
Для этого тексту задавалось свойство display:table. А для IE zoom:1.
<h3>overflow:hidden magic</h3>
Относительно недавно (относительно пяти лет) мы столкнулись с новым способом, оказалось что overflow:hidden может повторить этот эффект, и <a href="http://cssing.org.ua/examples/overflow-hidden/">сделать его даже лучше</a>. Причина обоих трюков, вовсе не глюки браузеров или специфика их отображения. Причина на сайте W3C:
<blockquote>The border box of a table, a block-level replaced element, or an element in the normal flow that establishes a new block formatting context (such as an element with ‘overflow’ other than ‘visible’) must not overlap any floats in the same block formatting context as the element itself.
W3C, CSS 2.1</blockquote>
<cite><a href="http://www.w3.org/TR/CSS2/visuren.html#floats">источник</a></cite>
То есть это не хак, а документированное поведение. Всё дело в так называемом «контексте» или «контексте форматирования», такие правила как display и overflow создают этот контекст, и согласно правилам он (созданный контекст) не может пересекаться с флоатами. Что вобщем и происходит. В результате блок занимает все доступное пространство <em>кроме флоата</em>.
<blockquote>Floats, absolutely positioned elements, inline-blocks, table-cells, table-captions, and elements with 'overflow' other than 'visible' (except when that value has been propagated to the viewport) establish new block formatting contexts.</blockquote>
Как видим контекст можно создавать разными способами.

Важное отличие от display:table &#8212; <em>ширина блока</em>, я сделал <a href="http://cssing.org.ua/examples/overflow-hidden/index_text.html">специальный пример</a> чтобы было видно, чем часто был неудобен именно display:table. 

Именно это отличие позволяет делать с overflow более сложные вещи чем с display:table.
<p class="img con"><img src="http://cssing.org.ua/pic/overflow/tablehidden.png" width="460" height="307" /><span>Когда мало текста, блок не занимает всю ширину</span></p>
<h3>IE?</h3>
<strong>IE6</strong> &#8212; не работает  ни display:table ни overflow:hidden. Нужно использовать zoom:1; (или любой hasLayout). В результате эффект идентичен действию overflow в других браузерах. 

<strong>IE7-8</strong> &#8212; overflow:hidden работает также как во всех остальных возможных браузерах.

Резюмируя: можно добавить к overflow:hidden еще zoom:1; и забыть о проблеме.
<h3>Возможные применения</h3>
Самое простое и банальное, вёрстка <a href="http://cssing.org.ua/examples/overflow-hidden/index_pic.html">блоков с текстом и картинкой</a>:
<p class="img con"><img src="http://cssing.org.ua/pic/overflow/2.png" width="377" height="149" /><span>Редкий сайт обходится без такого блока</span></p>
Используя overflow:hidden можно их стилизовать для произвольной ширины картинок.

Чуть более сложный кейс, <a href="http://cssing.org.ua/examples/overflow-hidden/index_input.html">резиновый инпут и кнопка</a>:
<p class="img con"><a href="http://cssing.org.ua/examples/overflow-hidden/"><img src="http://cssing.org.ua/pic/overflow/input.png" width="387" height="39" /><span>Обычное дело  на резиновых сайтах</span></a></p>
С подобной проблемой недавно столкнулся Глеб Арестов и <a href="http://friendfeed.com/yodapunk/c1ada988">успешно решил</a> её как раз с помощью этого же свойства.

Более  того, можно строить layout страниц. В частности в фреймворке <a href="http://wiki.github.com/stubbornella/oocss/">OOCSS</a> колонки строятся как раз с использованием этого свойства. Примерно так:
<p class="img con"><a href="http://cssing.org.ua/examples/overflow-hidden/index_layout.html"><img src="http://cssing.org.ua/pic/overflow/layout.png" width="456" height="99" /><span>Можно не задавать ширину резиновой колонке</span></a></p>
Конечно, тут минимум два недостатка. Во-первых, порядок контента &#8212; средняя колонка должна идти в коде после обоих боковых. Во-вторых, нестабильность при сжатии, когда что-то начинает не помещаться в блоке с overflow:hidden, его самым невероятным образом разрывает на части в IE. min-width мог бы спасти. <a href="http://cssing.org.ua/examples/overflow-hidden/index_layout.html">Использовать</a> осторожно.

Но, помнить о таком мощном приеме стоит.
<h3>Еще</h3>
<ul>
<li><a href="http://www.gunlaug.no/contents/wd_example_01_01.html">Пост Gunlaug</a> про это же поведение</li>
<li><a href="http://cssing.org.ua/2005/07/03/display-table/">Мой пост про display:table</a></li>
<li><a href="http://cssing.org.ua/examples/overflow-hidden/">Мой простой пример</a>, <a href="http://cssing.org.ua/examples/overflow-hidden/index_layout.html">пример трехколоночного сайта</a></li>
<li><a href="http://flack.ru/2008/08/26/semantic-coding-howto-6/">Пост Flack на эту же тему</a></li>
<li><a href="http://habrahabr.ru/blogs/css/48383/">Clear или overflow:hidden — очистка всего потока или создание контекста форматирования?</a></li>
<li><a href="http://habrahabr.ru/blogs/css/48429/">Управление потоком в CSS: создаём контекст форматирования</a></li>
</ul>
Это не CSS3 и далеко не вчерашнее изобретение, но кажется многие недооценивают силу этого простого приема.

Буду рад если поделитесь своим опытом!
