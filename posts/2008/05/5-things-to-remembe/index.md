---
title: "5 советов верстальщику"
date: "2008-05-21"
humanDate: "21 May, 2008"
permalink: "2008/05/21/5-things-to-remembe/"
tags: 
  - "xhtmlcss"
  - "common"
comments: 
  -  author: "Равномерный фон под текстом &laquo; PHP Portal"
     id: "15260"
     url: "http://kobzarev.com:80/hack/uniform-text-background.html"
     date: "2010-01-24 16:44:42"
     humandate: "24 Jan, 2010"
     content: | 
       [...] всех к решению задачи когда-то подошёл akella, добавив border у родительского элемента. Но проблема не [...]

     email: ""

  -  author: "Равномерный фон под текстом"
     id: "15163"
     url: "http://chikuyonok.ru/2010/01/uniform-text-background/"
     date: "2010-01-19 16:37:30"
     humandate: "19 Jan, 2010"
     content: | 
       [...] всех к решению задачи когда-то подошёл akella, добавив border у родительского элемента. Но проблема не [...]

     email: ""

  -  author: "Глеб"
     id: "14766"
     url: "http://133th.livejournal.com"
     date: "2009-09-07 02:55:28"
     humandate: "07 Sep, 2009"
     content: | 
       Привет, а почему в первом не сделать так:
       
       &lt;h1 id="logo"&gt;&lt;a href="#"&gt;!&lt;span&gt;Вау! Я логотип&lt;/span&gt;&lt;/a&gt;&lt;/h1&gt;
       
       #logo a {
        dispay:block;
        width:250px;
        height:250px
        background:url(img.gif);
       }
       
       #logo a span {
        display:none;
       }

     email: "133gl@bk.ru"

  -  author: "akella"
     id: "14768"
     url: "http://cssing.org.ua"
     date: "2009-09-07 10:31:50"
     humandate: "07 Sep, 2009"
     content: | 
       Это чтобы при отключенных картинках было видно текст

     email: "akella.a@gmail.com"

  -  author: "Иван Маркеев"
     id: "12446"
     url: "http://markeev.labwr.ru"
     date: "2008-05-22 06:22:56"
     humandate: "22 May, 2008"
     content: | 
       Заметка во многом спорная. "смешные имена классам и айди", как и "Использовать табуляцию в CSS" справедливо если деплоймент и девелопмент версии CSS-ок и HTML-ек отличаются. Если нет, то страница сильно потяжелеет. И собственно зачем? Чтоб программистов повеселить? А обычные юзверы будут тыкатся на неоптимизированный сайт?
       
       На счет колдвства с в самом начале у меня тоже хватает опасений. Семантика при таком подхлоде не страдает? Я просто не уверен, что такое колдунство будет правильно ботом воспринято.
       
       А вообще, понимаю, что заметка не мне, а Виталию Харисову и др., так что больше настроение не порчу.

     email: "markeev@labwr.ru"

  -  author: "akella"
     id: "12447"
     url: "http://cssing.org.ua"
     date: "2008-05-22 08:36:24"
     humandate: "22 May, 2008"
     content: | 
       Да портьте на здоровье! :) Я за здоровую критику всегда!
       Пустой спан это вред семантике? Чему кроме рафинированно-идеологического восприятия кода он может навредить? Известен ли вам лучший способ заменять текст картинками? С удовольствием заменю в посте и буду сам использовать.
       Ботам на данный момент все равно, да и почему им вообще должно быть дело до пустого спана.
       
       &gt;А обычные юзверы будут тыкатся на неоптимизированный сайт?
       При всем уважении, я не могу относиться серьезно к утяжелению сайта на 50 байт. Разумеется если мы будем верстать сайт яндекса, или майкрософта, можно и поэкономить. Но 99% будут иметь посещаемость и баннеры, на фоне которых это как-то даже несерьезно :)
       
       Если уж так важна оптимизация, можно удалять табы при деплойменте, или в своем текстовом редакторе перед отсылкой. Но нельзя забывать об ускорении разработки что они дают. Это порой гораздо важнее чем аж 1-2 килобайта лишнего CSS. (которые еще потом нужно поделить на 5 засчет gzip) Я тоже очень люблю все оптимизировать, но надо во всем знать меру, ИМХО. 
       Иначе спойлер на машины ставить станет нерационально :) толку от него? Только машина тяжелее.
       
       Спасибо за критику! Заметка не кому-то конкретно, а всем. Буду рад поспорить по поводу неё.
       Ну и, нельзя же так серьезно ко всему относиться ;)

     email: "akella.a@gmail.com"

  -  author: "macgera"
     id: "12448"
     url: "http://www.macgera.name"
     date: "2008-05-22 11:14:53"
     humandate: "22 May, 2008"
     content: | 
       Я вот, например, табуляцию вверстке вообще терпеть не могу. Не знаю...
       
       Но вот 5-й совет. Я себе его постоянно в голове напоминаю когда хочется поднять руку и "........." :)

     email: "macgera@gmail.com"

  -  author: "Андрей.П"
     id: "12449"
     url: ""
     date: "2008-05-22 11:41:02"
     humandate: "22 May, 2008"
     content: | 
       А зачем такие жестокие манипуляции для замены текста картинкой? 
       Только для тех, кто выключает отображение картинок в браузере, забыв выключить цсс?

     email: "nyctota@hws.ru"

  -  author: "акелла"
     id: "12450"
     url: "http://cssing.org.ua"
     date: "2008-05-22 11:56:54"
     humandate: "22 May, 2008"
     content: | 
       Именно для тех кто вырубает картинки. Я сторонник качества. Качество всегда оплачивается.
       И нормальные заказчики с вас рано или поздно такое спросят.
       
       А табуляция как я и говорил на любителя. Пока не попробовал вызывала только отвращение :)

     email: "akella.a@gmail.com"

  -  author: "Zigzag"
     id: "12452"
     url: "http://webdev.lovata.com"
     date: "2008-05-22 13:05:37"
     humandate: "22 May, 2008"
     content: | 
       Всеобщее безумие =)

     email: "zigzag.mcquack@gmail.com"

  -  author: "Свобода слова"
     id: "12453"
     url: "http://spamparampampam.com/"
     date: "2008-05-22 18:05:34"
     humandate: "22 May, 2008"
     content: | 
       Спасибо за советы. Пригодятся. )

     email: "4317295@gmail.com"

  -  author: "Octane"
     id: "12455"
     url: "http://www.webpp.ru"
     date: "2008-05-22 22:15:58"
     humandate: "22 May, 2008"
     content: | 
       А не лучше ли в первом пункте для ссылки указать position: releative, а для вложенного span'a top:0 и left:0; тогда не нужно будет задумываться о координатах вообще. Такую технику применил в моей работе http://www.fabrichny.ru для оформления кнопок навигации, работает в IE5+ (для проектов не масштаба поисковых систем и социальных сервисов такой совместимости вполне достаточно я думаю) и в любых других нормальных браузерах.

     email: "paagrio@list.ru"

  -  author: "Vitaly Harisov"
     id: "12457"
     url: "http://vitaly.harisov.name"
     date: "2008-05-22 23:26:18"
     humandate: "22 May, 2008"
     content: | 
       <a href="http://harisov.livejournal.com/105323.html" rel="nofollow">Написал свои</a>.

     email: "vitaly@harisov.name"

  -  author: "akella"
     id: "12458"
     url: "http://cssing.org.ua"
     date: "2008-05-22 23:39:10"
     humandate: "22 May, 2008"
     content: | 
       @Octane: не совсем понял, у меня же тоже самое написано?
       
       Залинковал на Вас, Виталий!

     email: "akella.a@gmail.com"

  -  author: "Octane"
     id: "12459"
     url: "http://www.webpp.ru"
     date: "2008-05-22 23:58:49"
     humandate: "22 May, 2008"
     content: | 
       ыыы и правда :-[ ступил чот, пойду высплюсь )))

     email: "paagrio@list.ru"

  -  author: "Mons"
     id: "12460"
     url: "http://blog.mons.ws"
     date: "2008-05-23 11:39:51"
     humandate: "23 May, 2008"
     content: | 
       Смешные названия, радуют не только программистов но и поисковики :)

     email: "rewe@mail.ru"

  -  author: "Грешник"
     id: "12461"
     url: "http://mysin.ru"
     date: "2008-05-23 12:09:41"
     humandate: "23 May, 2008"
     content: | 
       Табуляция ИМХО лишь затягивает процесс работы

     email: "mysin@mysin.ru"

  -  author: "Олег"
     id: "12464"
     url: "http://spamparampampam.com/"
     date: "2008-05-26 12:01:20"
     humandate: "26 May, 2008"
     content: | 
       Спс, так как я только учусь, очень познавательная статья для меня, еще рас спасибо.

     email: "objectives@inbox.ru"

  -  author: "янеробот"
     id: "12466"
     url: "http://www.uzb.ru"
     date: "2008-05-26 23:20:37"
     humandate: "26 May, 2008"
     content: | 
       Эти советы даны человеком с большим чувством юмора:))) и это хорошо, позитив он всегда в плюсе!

     email: "pioriko@mail.ru"

  -  author: "Андрей.П"
     id: "12467"
     url: ""
     date: "2008-05-26 23:33:36"
     humandate: "26 May, 2008"
     content: | 
       Только понял: такая техника замены текста картинкой имеет негативный эффект — лого не поместить на неоднородный фон. 
       
       И еще, с учетом того, что размеры лого как правило небольшие, а заголовок первого уровня все-таки довольно крупный по размеру, врядли что-то осмысленное будет написано в окошечке, появившемся на месте лого, если пользователь выключит картинки.

     email: "nyctota@hws.ru"

  -  author: "akella"
     id: "12468"
     url: "http://cssing.org.ua"
     date: "2008-05-27 00:18:09"
     humandate: "27 May, 2008"
     content: | 
       Верстку логотипа я скорее в качестве примера, а размер текста для него можно указать и маленький - тогда он отобразиться как обычная ссылка вверху :) И все поместится.
       Насчет фона - да, есть такой дело, случается редко, и лучше в таких случаях применять Thierry Image Placement из <a href="http://cssing.org.ua/2006/02/23/image-replacement/" rel="nofollow">этого поста</a>

     email: "akella.a@gmail.com"

  -  author: "/Н.П.Блок/ &raquo; &raquo; 5 советов IT-специалисту на примере вёрстки"
     id: "12469"
     url: "http://blog.netpro.ru/index.php/2008/05/27/5-sovetov-it-specialistu-na-primere-vyorstki/"
     date: "2008-05-27 11:20:16"
     humandate: "27 May, 2008"
     content: | 
       [...] советов по вёрстке добралась и до меня (спасибо Юре Артюху) - с удовольствием ими поделюсь. Данные советы [...]

     email: ""

  -  author: "Konstantin"
     id: "12470"
     url: ""
     date: "2008-05-27 11:28:43"
     humandate: "27 May, 2008"
     content: | 
       1. Правильная замена на картинки
       
       в примере с логотипом или в случаях когда имеем дополнительный тег в блоке, есть еще одна техника, которая редко упоминается - задание opacity.
       
       3. Выделенный текст
       
       я бы сделал h2 - position:relative и span - position:absolute. так легче позицировать текст и нет необходимости задавать бордер для h2.
       
       4. Относитесь к вёрстке с чувством юмора
       
       только не материтесь в коде :)

     email: "volgin.k@gmail.com"

  -  author: "akella"
     id: "12472"
     url: "http://cssing.org.ua"
     date: "2008-05-27 13:12:27"
     humandate: "27 May, 2008"
     content: | 
       1. Вы имеете ввиду задание opacity для текста? Но ведь тогда его не будет видно при отключенных картинках? Разве нет?
       
       2. Но ведь тогда текст будет выглядывать справа от заголовка? Ведь паддинги не учитывают справа, как видно по картинки.

     email: "akella.a@gmail.com"

  -  author: "webmolot"
     id: "12473"
     url: "http://www.webmolot.com"
     date: "2008-05-27 16:16:17"
     humandate: "27 May, 2008"
     content: | 
       Мои 5 советов по html/css верстке сайтов.
       
       1. Если ты уделяешь верстке 1 час в день - не жди успеха. Если за версткой ты не замечаешь как летит время, можешь работать целый день и это приносит удовольствие - значит ты верстальщик-фанатик, и со временем ты сможешь верстать как твои кумиры.
       
       2. Не останавливайся на достигнутом! Читай больше статей про html/css верстку. Броди по блогам верстальщиков, там можно найти много новой и полезной для себя информации. Все знать ты не можешь.
       
       3. Собирай и структурируй свою библиотеку решений по верстке и создавай свои фреймворки. Это поможет сэкономить много времени при верстке.
       
       4. Таблицы используй только для вывода табличных данных. Не слушай тех, кто говорит, что таблицами верстать быстрее и надежнее. Это говорят ленивые верстальщики, которые выучили 5 лет назад табличную верстку (тогда она была актуальной), а сейчас не хотят переучиваться. Грамотная блочная верстка справится с макетами любой сложности!
       
       5. Не напрягай мозг, заучивая новые теги, приемы и технологии верстки. Не обязательно все помнить и держать в голове, важнее знать, где это найти в случае необходимости! Если ты будешь много верстать - все это само сабой отложится в памяти.

     email: "webmolot@gmail.com"

  -  author: "cyrillyun"
     id: "12477"
     url: "http://cyrillyun.blogspot.com"
     date: "2008-05-27 23:06:44"
     humandate: "27 May, 2008"
     content: | 
       "Помни про носовой платок и не выходи без галош"? :)

     email: "kirill.yun@gmail.com"

  -  author: "cyrillyun"
     id: "12478"
     url: "http://cyrillyun.blogspot.com"
     date: "2008-05-27 23:17:47"
     humandate: "27 May, 2008"
     content: | 
       2webmolot: продолжу ваши советы в контексте программирования
       
       6. Не используйте goto. Не слушайте тех, кто говорит о большем удобстве программирования с этим оператором - ваш код будет запутанным и сложным для сопровождения 
       
       7. Комментируйте ваш код. 
       
       ...думаю, смысл понятен :)

     email: "kirill.yun@gmail.com"

  -  author: "Павел"
     id: "12479"
     url: "http://www.amazedev.com"
     date: "2008-05-27 23:55:01"
     humandate: "27 May, 2008"
     content: | 
       Написал свои 5 советов 
       http://www.amazedev.com/5-sovetov-verstalshhiku/
       Как в тостах на День Рожденье счастье, здоровье и успехов разбирают первые поздравляющие :)

     email: "amazedev@gmail.com"

  -  author: "Troppus"
     id: "12480"
     url: ""
     date: "2008-05-28 10:01:41"
     humandate: "28 May, 2008"
     content: | 
       Использую такой вариант для подмены текста картинкой (проблем с поисковыми ботами ни разу не было за последние 5 лет меня в блочной верстке):
       
       &lt;h1title=&quot;Вау! Я логотип!&quot;&gt;&lt;a href=&quot;#&quot;&gt;&lt;span&gt;Вау! Я логотип!&lt;/span&gt;&lt;/a&gt;&lt;/h1&gt;
       
       h1, h1 a { display: block; margin: 0; padding: 0; width: 100px; height: 100px }
       h1 { background: transparent url(/images/kartinka.png) no-repeat }
       h1 a span { display: none }
       
       :-)

     email: "troppus@gmail.com"

  -  author: "akella"
     id: "12482"
     url: "http://cssing.org.ua"
     date: "2008-05-28 10:51:53"
     humandate: "28 May, 2008"
     content: | 
       Отличный вариант! Я его не использую только из-за того, что при отключенных картинках мы ничего не увидим. Но вариант один из самых надежных.

     email: "akella.a@gmail.com"

  -  author: "Troppus"
     id: "12483"
     url: ""
     date: "2008-05-28 12:29:05"
     humandate: "28 May, 2008"
     content: | 
       Кстати, верное замечание. Можно конечно к данному XHTML коду применить другой подход, где в этой же конструкции span будет участвовать как тег с absolute позиционированием на фоне остальных h1- и a- тегов с static позиционированием, но увы именно c FF под Win возникает проблема с отображением span-a при z-index: -1 и hidden: overflow (в том же FF1.x, 3.0/Safari под Mac проблем нет). Т.е. без дополнительного вмешательства в код не получится, значит этот вариант отпадает :-)
       К слову об отключенных картинках, процент таких посетителей ниже или равен проценту использования пользователями Safari for Mac в мировом масштабе.
       Тут необходимо четко разделять, для какой аудитории предназначается ресурс и какие трудности могут возникнуть в применении очередного стиля при неизменном XHTML коде. Иногда бывает очень целесообразным (с точки зрения совместимости умирающего IE6) применения вот такого XHTML кода:
       
       &lt;h1 title=&quot;Вау! Я логотип!&quot;&gt;&lt;a href=&quot;#&quot;&gt;&lt;img src=&quot;images/kartinka.png&quot; alt=&quot;Вау! Я логотип!&quot; width=&quot;100&quot; height=&quot;100&quot; border=0 /&gt;&lt;/a&gt;&lt;/h1&gt;
       
       Как ни банально. Не судите строго :-)

     email: "troppus@gmail.com"

  -  author: "akella"
     id: "12485"
     url: "http://cssing.org.ua"
     date: "2008-05-28 13:28:39"
     humandate: "28 May, 2008"
     content: | 
       не совсем понял о каких проблемах с z-index:-1 вы говорите. Вот у меня ж как раз первый метод такой, который работает при отключенных картинках во всех броузерах, включая ИЕ5-8, и использует z-index.
       Может быть есть пример этой техники? Было бы интересно.

     email: "akella.a@gmail.com"

  -  author: "Troppus"
     id: "12486"
     url: ""
     date: "2008-05-28 16:32:09"
     humandate: "28 May, 2008"
     content: | 
       Это понятно, что первый пример будет работать везде при исходной конструкции XHML кода, но хотелось бы обойтись без пустых тегов.
       
       Эту технику (см.ниже) можно использовать в отдельных случаях, но повторюсь, что в FF под Windows она не заработала (может быть у Вас получится).
       
       h1, h1 a, hi a span { display: block; margin: 0; padding: 0; width: 100px; height: 100px }
       h1 a span { width: 100px; height: 100px; position: absolute; z-index: -1; font-size: medium; overflow: hidden }
       h1 { background: url(/images/kartinka.png) no-repeat }
       
       повторное задание размеров необходимо, чтобы код корректно отрабатывался под FF/Safari for Mac.

     email: "troppus@gmail.com"

  -  author: "Troppus"
     id: "12487"
     url: ""
     date: "2008-05-28 16:39:32"
     humandate: "28 May, 2008"
     content: | 
       Извиняюсь, вышла опечатка в "h1 a span" :-)
       
       Вот немного измененный код:
       
       h1, h1 a, h1 a span { display: block; margin: 0; padding: 0; width: 100px; height: 100px }
       h1 a span { position: absolute; z-index: -1; font-size: medium; overflow: hidden }
       h1 { background: url(/images/kartinka.png) no-repeat }
       
       Но все равно он не корректно работает в FF под Win.

     email: "troppus@gmail.com"

  -  author: "Troppus"
     id: "12488"
     url: ""
     date: "2008-05-28 16:48:50"
     humandate: "28 May, 2008"
     content: | 
       А вот авторский CSS можно немного оптимизировать и привести к такому виду:
       
       h1 a, h1 a span { width:250px;height:50px; overflow:hidden; display:block }
       h1 a span { position:absolute; background:transparent url(../img/kartinka.png) no-repeat 0 0 }
       
       из "h1 a" была убрана релативность в позиционировании, т.к. в данном случае она не нужна как и не нужны "top: 0" и "left: 0" в "h1 a span". Проверьте, думаю визуализация будет везде одинаковая. :-)

     email: "troppus@gmail.com"

  -  author: "dv"
     id: "12490"
     url: "http://vozniy.com"
     date: "2008-05-28 17:56:57"
     humandate: "28 May, 2008"
     content: | 
       Спасибо за советы, Пригодятся. )

     email: "dv_go@ua.fm"

  -  author: "akella"
     id: "12492"
     url: "http://cssing.org.ua"
     date: "2008-05-28 20:48:56"
     humandate: "28 May, 2008"
     content: | 
       @Troppus: Зная что такое Опера и ИЕ5 я так не люблю рисковать :) Нужно тестировать...
       
       <strong>Update</strong>: В сафари не пашет упрощение... =( Так что прийдется писать длиннее...

     email: "akella.a@gmail.com"

  -  author: "Troppus"
     id: "12501"
     url: ""
     date: "2008-05-29 18:03:44"
     humandate: "29 May, 2008"
     content: | 
       2akella: увы, по той же статистике пользователей Opera и IE5.x в сумме одинаково столько же сколько пользователей Safari (~2.5%). Поэтому риск тут минимальный.
       
       Вот кстати, браузерная статистика для общей информации (если интересно):
       http://www.w3schools.com/browsers/browsers_stats.asp
       
       Но могу сказать и обратное, в моей практике встречаются очень крупные проекты, ресурсы которых исчисляются миллионами и десятками миллионами уникальных посещений в день - тогда даже десятую долю процента браузерной статистики нужно учитывать. :-)
       
       Важно понимать под какую аудиторию предназначается конкретный ресурс. Отнюдь не лень, а холодный расчет, но это работает и экономит нам разработчикам время и силы, дамы и господа!
       
       P.S. А Вы под каким Safari тестировали (версия и платформа) и что именно не корректно отображалось?

     email: "troppus@gmail.com"

  -  author: "Andrey"
     id: "12496"
     url: "http://spamparampampam.com/"
     date: "2008-05-29 11:58:41"
     humandate: "29 May, 2008"
     content: | 
       Спасибо за советы

     email: "admin@kpoxa.cn"

  -  author: "akella"
     id: "12502"
     url: "http://cssing.org.ua"
     date: "2008-05-29 18:07:46"
     humandate: "29 May, 2008"
     content: | 
       Безусловно, я знаком со статистикой :) Спасибо. Но ваше к ней отнношение радикально меняется когда ваш основной броузер принадлежит к тем же 2.5%.
       
       Насчет статистики согласен, но в данном случае трудозатраты по поддержке этой пары процентов, довольно просты..
       
       
       Я смотрел под Safari 3.1.1, Mac OS X 10.5.2.
       Абсолютно спозиционированный спан с фоном, отобразился сбоку от текста. 
       Вообще есть ведь даже такой клевый прием эксплуатирующий это, абсолютные элементы отображаются под последними статическими, при неуказанных координатах.

     email: "akella.a@gmail.com"

  -  author: "Troppus"
     id: "12507"
     url: ""
     date: "2008-05-29 21:15:39"
     humandate: "29 May, 2008"
     content: | 
       Верно, значит нужно изменить местоположение span-тега в пределах a-тега :-)
       
       &lt;h1&gt;&lt;a href=&quot;#&quot;&gt;&lt;span&gt;&lt;/span&gt;Вау! Я логотип!&lt;/a&gt;&lt;/h1&gt;
       
       По поводу "Оперной" аудитории Вы правы - если ресурс считается с этой аудиторией, тогда безусловно это принимается во внимание, я лишь привёл общую статистику по всему интернету. :-)

     email: "troppus@gmail.com"

  -  author: "Юлия"
     id: "12536"
     url: "http://spamparampampam.com/"
     date: "2008-06-02 08:09:39"
     humandate: "02 Jun, 2008"
     content: | 
       Неплохие советы, но самый важный, я считаю, про то что нужно использовать табуляцию. Вообще в идеале она нужна везде, ведь так проще найти, если чтото не так да и вообще проще понять код.

     email: "rapbrothers01@yandex.ru"

  -  author: "ПаЛыЧ"
     id: "12565"
     url: "http://palpalych.ru"
     date: "2008-06-03 10:25:23"
     humandate: "03 Jun, 2008"
     content: | 
       Я бы добавил про не забываем закрывать атрибуты.

     email: "ya@palpalych.ru"

  -  author: "YoYurec"
     id: "12567"
     url: "http://yoyurec.in.ua"
     date: "2008-06-03 14:10:04"
     humandate: "03 Jun, 2008"
     content: | 
       по поводу замены картинкой (ссылка в span) - http://neal.venditto.org/nir.php, почти как у автора. работает везде на ура!
       метод прохродит все тесты (http://wd.mrclay.org/tests/ir/), собсно как и знатный A.Levin's IR...

     email: "yoyurec@gmail.com"

  -  author: "akella"
     id: "12581"
     url: "http://cssing.org.ua"
     date: "2008-06-04 18:20:06"
     humandate: "04 Jun, 2008"
     content: | 
       Спасибо! Замечательный метод =) Жаль что не очень популярный был раньше, буду теперь его применять =)

     email: "akella.a@gmail.com"

  -  author: "Уроки верстки – CSS подмена текста картинкой :: Дизайн Мания"
     id: "14480"
     url: "http://design-mania.ru/web-design/html-css/css-podmena/"
     date: "2009-06-10 01:07:33"
     humandate: "10 Jun, 2009"
     content: | 
       [...] можно наблюдать у варианта номер 2 под названием правильная замена на картинки. &lt;h1&gt;&lt;a href=&quot;#&quot;&gt;Вау! Я [...]

     email: ""

  -  author: "Серега"
     id: "12630"
     url: "http://spamparampampam.com/"
     date: "2008-06-12 16:59:15"
     humandate: "12 Jun, 2008"
     content: | 
       Спасибо за советы, особенно порадовал последний - доведите верстку до конца. )

     email: "kolsergio@ya.ru"

  -  author: "Алекс"
     id: "12632"
     url: "http://spamparampampam.com/"
     date: "2008-06-12 22:13:37"
     humandate: "12 Jun, 2008"
     content: | 
       CSS-техники увы сложноваты, но конечно же без них никуда.

     email: "pioriko@mail.ru"

  -  author: "bong-bong"
     id: "12669"
     url: "http://spamparampampam.com/"
     date: "2008-06-21 11:02:47"
     humandate: "21 Jun, 2008"
     content: | 
       Без CSS сейчас никуда, табличная верстка давно устарела. Дивы рулят ;)

     email: "zheran@list.ru"

  -  author: "Алекс"
     id: "12703"
     url: "http://spamparampampam.com/"
     date: "2008-06-24 13:52:37"
     humandate: "24 Jun, 2008"
     content: | 
       Отличные советы, сасибо огромные я только начинаю заниматься этим, так что мне будет полезно это знать!

     email: "arkaha83@inbox.ru"

  -  author: "Олег"
     id: "12707"
     url: "http://spamparampampam.com/"
     date: "2008-06-24 22:50:06"
     humandate: "24 Jun, 2008"
     content: | 
       Очень понравился первый пример, как-то о таком приеме даже не задумывался.
       А на счет табличной верстки я бы не стал говорить что она устарела. Иногда с ней сделать все намного проще и быстрее, чем с div'ами.

     email: "bar-boss2008@mail.ru"

  -  author: "Gan"
     id: "12809"
     url: "http:"
     date: "2008-07-09 14:06:20"
     humandate: "09 Jul, 2008"
     content: | 
       не могу понять первый совет! В чем фишка?
        Например если отключить картинку, а у картинки написать альт, то также надпись будет появляться при отключении картинок! Предпалогаю это все для того что бы при отключении именно ксс появлялась надпись замест логотипа! Если это все для этого то знаю еще один способ! Это ставить свойство text-indent:-9999px для ссылки которая в логотипе!

     email: "slangpro@yahoo.com"

  -  author: "Gan"
     id: "12812"
     url: "http://yvelious.com"
     date: "2008-07-09 14:27:42"
     humandate: "09 Jul, 2008"
     content: | 
       Хотя конечно это будет не сильно удобно! так как при отключении именно картинки не хрена не видино будет

     email: "slangpro@yahoo.com"

  -  author: "Никс"
     id: "12813"
     url: "http://www.maurit.ru"
     date: "2008-07-09 16:51:36"
     humandate: "09 Jul, 2008"
     content: | 
       Скажем точне это будет совсем неудобно, но другого выхода более приемлимого наверное нет.

     email: "swanspark@mail.ru"

  -  author: "NikNAME"
     id: "13151"
     url: "http://spamparampampam.com/"
     date: "2008-08-27 19:32:59"
     humandate: "27 Aug, 2008"
     content: | 
       Спасибо большое...Я в ксс очень плохо разбираюсь...мой кот куда лучше наверно))Так вот статья помогла я понял хотьь базовые приёмы...возьму эту статью на заметку!

     email: "FSWB@yandex.ru"

  -  author: "Борис"
     id: "13158"
     url: "http://google.com"
     date: "2008-08-29 15:37:12"
     humandate: "29 Aug, 2008"
     content: | 
       Понравился совет доводить вёрстку до конца

     email: "boriska@mail.com"

  -  author: "Мегабайтыч"
     id: "13629"
     url: "http://saydesign.ru"
     date: "2008-11-19 20:07:54"
     humandate: "19 Nov, 2008"
     content: | 
       Олег,и не так геморно с кроссбраузерностью.
        Однако думается в скором времени браузеры доведут до ума,и таблицы уйдут туда,где им место

     email: "rebenn@yandex.ru"

  -  author: "akella"
     id: "14018"
     url: "http://cssing.org.ua"
     date: "2009-01-30 15:35:23"
     humandate: "30 Jan, 2009"
     content: | 
       Попробуйте добавить такую строку
       a:hover{background:url(whatever.png) no-repeat 0 0}

     email: "akella.a@gmail.com"

  -  author: "Viktor"
     id: "14019"
     url: ""
     date: "2009-01-30 21:26:10"
     humandate: "30 Jan, 2009"
     content: | 
       попробовал метод http://neal.venditto.org/nir.php , у меня текст ссылки больше логотипа и в IE7 вылазит за пределы лого... и соответственно его видно... как быть?

     email: "nk2006@gmail.com"

  -  author: "Сергей"
     id: "14017"
     url: ""
     date: "2009-01-30 13:55:07"
     humandate: "30 Jan, 2009"
     content: | 
       Попробовал применить ваш метод с заменой текста на картинки в меню, т.е. по умолчанию одна картинка, а при наведении другая. В IE6 при на ведении курсора появляется нужная картинка и так там и остается висеть даже когда курсор убрать. Короче пока старницу не перегрузишь, она не уберется. Подскажите как это обойти?

     email: "chumak.sergei@gmail.com"

  -  author: "akella"
     id: "14021"
     url: "http://cssing.org.ua"
     date: "2009-01-31 10:11:53"
     humandate: "31 Jan, 2009"
     content: | 
       Не нужно использовать другой метод просто добавьте мою строку к старому.
       
       Попробуйте еще overflow:hidden

     email: "Akella.a@gmail.com"

  -  author: "Сергей"
     id: "14022"
     url: ""
     date: "2009-02-01 11:28:39"
     humandate: "01 Feb, 2009"
     content: | 
       2akella: Спасибо за совет, помогло. Решение, как всегда, оказалось проще некуда :)

     email: "chumak.sergei@gmail.com"

  -  author: "5 вредных советов верстальщику"
     id: "18784"
     url: "http://www.fortress-design.com/layout/5-vrednyx-sovetov-verstalshhiku/"
     date: "2010-08-29 03:14:46"
     humandate: "29 Aug, 2010"
     content: | 
       [...] эстафету от Акеллы. Полный список тех кому нечего делать [...]

     email: ""

  -  author: "Дмитрий"
     id: "18773"
     url: ""
     date: "2010-08-19 01:09:03"
     humandate: "19 Aug, 2010"
     content: | 
       Статья - тотальный и беспрецедентный бред! Вот из-за таких "верстальщиков", которых очень тянет к обучению других таких же, рынок наполняется быдлокодерами! Поучи сначала алгоритмы работы поисковиков, браузеров и рекомендации W3C по назначению определенных тегов, потом добавь к этому здравый смысл и удали эту статью!

     email: "vi_rus@list.ru"

  -  author: "Веб-дизайн &raquo; Архив блога &raquo; Уроки верстки – CSS подмена текста картинкой"
     id: "25644"
     url: "http://onlinokino.ru/?p=301"
     date: "2011-11-16 16:05:27"
     humandate: "16 Nov, 2011"
     content: | 
       [...] В комментариях к этой реализации посоветовали добавить опцию overflow:hidden чтобы «при увеличении шрифта снизу ничо не полезло». Нечто подобное можно наблюдать у варианта номер 2 под названием правильная замена на картинки. [...]

     email: ""

  -  author: "Евгений"
     id: "31159"
     url: "http://www.beskrovnyy.com/"
     date: "2011-12-30 01:14:30"
     humandate: "30 Dec, 2011"
     content: | 
       А курсорчик в виде ручечки, для иешечки на спанчике в логотипчике? :)

     email: "e.beskrovnyy@gmail.com"

  -  author: "Советы верстальщикам | Web Sphere Blog"
     id: "60364"
     url: "http://websphere.netau.net/?p=22"
     date: "2012-06-01 13:04:14"
     humandate: "01 Jun, 2012"
     content: | 
       [...] * Юрий Артюх [...]

     email: ""

layout: "layouts/post.njk"
excerpt: "Принимаю <a href=\"http://uggallery.audiopeace.ru/2008/05/19/5-advices\">всеобщее</a> <a href=\"http://blog.sribna.com/5-sovetov-verstalschiku.htm\">увлечение</a> рекомендациями по вёрстке. Мои 5 советов верстальщику. Не тайные манускрипты, а всего лишь простые советы :)"
---

Принимаю <a href="http://uggallery.audiopeace.ru/2008/05/19/5-advices">всеобщее</a> <a href="http://blog.sribna.com/5-sovetov-verstalschiku.htm">увлечение</a> рекомендациями по вёрстке. Мои 5 советов верстальщику. Не тайные манускрипты, а всего лишь простые советы :)<!--more-->
Я в этом блоге только тем и занимаюсь, что пытаюсь дать полезные советы, потому слегка повторюсь.
<h3>1. Правильная замена на картинки</h3>
Заменяйте текст на картинки хорошими CSS-техниками, например, для кликабельного логотипа сайта, нужен такой html:
<ol class="code">
<li>&lt;h1&gt;&lt;a href=&quot;#&quot;&gt;Вау! Я логотип!&lt;span&gt;&lt;/span&gt;&lt;/a&gt;&lt;/h1&gt;</li>
</ol>
CSS:
<ol class="code">
<li>h1 a{
<li class="tab">width:250px;height:50px;</li>
<li class="tab">overflow:hidden;</li>
<li class="tab">display:block;</li>
<li class="tab">position:relative;</li>
<li class="tab">}</li>
<li class="tab">h1 a span{</li>
<li class="tabtab">position:absolute;</li>
<li class="tabtab">width:250px;height:50px;</li>
<li class="tabtab">top:0;</li>
<li class="tabtab">left:0;</li>
<li class="tabtab">background:transparent url(../img/kartinka.png) no-repeat 0 0;</li>
<li class="tabtab">}</li>
</ol>
<h3>2. Использовать табуляцию в CSS</h3>
Суть в табулировании селекторов в зависимости от иерархии. Чем более "глубокий" элемент &#8212; тем большим кол-вом табов он будет отделен.
Это на любителя, но попробовать совершенно точно стоит. Живой пример этого видно чуть выше, а вот так это выглядит издалека и вживую:
<p class="img con"><img src="http://cssing.org.ua/pic/tabsbabs.png" alt="табулияция в CSS" /><span>Мне нравится. 
Как видно, иногда я пишу правила в одну строку, особенно когда подряд идут несколько правил с указанием лишь background</span></p>
<h3>3. Выделенный текст</h3>
Очень простой и маленький приём. Иногда полезен.
Вот такой код:
<ol class="code">
<li>&lt;h2&gt;&lt;span&gt;Ищу ту, особенную!&lt;/span&gt;&lt;/h2&gt;</li>
</ol>
В дизайне дано такое:
<p class="img"><img src="http://cssing.org.ua/pic/50c1.png" alt="выделенный текст" /><span>Выделенный красным "маркером" текст</span></p>
Если попробовать решать задачу "в лоб", пишем такое:
<ol class="code">
<li>h2 span{background:red;padding:4px;}</li>
</ol>
получаем это:
<p class="img"><img src="http://cssing.org.ua/pic/50c2.png" alt="выделенный текст" /><span>Вторая строка "прилипает" к краю. 
Мелочь, а неприятно</span></p>
Вариантов решения несколько, наиболее простой таков:
<ol class="code">
<li>h2{<strong>border-left:4px solid red</strong>;}</li>
<li>h2 span{background:red;padding:4px 4px 4px <strong>0</strong>;}</li>
</ol>
Результат:
<p class="img"><img src="http://cssing.org.ua/pic/50c1.png" alt="выделенный текст" /><span>Правильно выделенный текст</span></p>
Я ранее решал этот вопрос повторением фонового рисунка и паддингом для H2. Подсказал <a href="http://mega.genn.org">genn</a>. 
<h3>4. Относитесь к вёрстке с чувством юмора</h3>
Например, можно давать смешные названия классам и айди.
Не стоит этим злоупотреблять, и использовать на сайтах где важна оптимизация, но на сайте какой-то веб-студии, или чисто представительском сайте это вполне оправдано:
<ol class="code">
<li>&lt;div class="i-was-born-in-1494"&gt;</li>
</ol>
Или
<ol class="code">
<li>&lt;div class="usually-i-dont-use-such-a-long-names-for-classes-but-today-is-a-special-day"&gt;</li>
</ol>
Могут сильно повеселить программистов и любителей заглянуть в ваш код. Смешной селектор может быть и коротким, главное, остроумным.

Желательно конечно, чтобы такой класс или айди встречался в коде лишь один раз. Впрочем, возможны варианты. :) Еще можно шутить прямо в CSS.

<h3>5. Доводите вёрстку до конца</h3>
Никогда не сдавайтесь на пол-пути в сложном проекте. Какими бы титаническими ни были усилия они практически всегда окупаются, если не деньгами то опытом и выносливостью. А так же духом победителя.
<h3>__END__</h3>
Адресую <a href="http://harisov.livejournal.com/">Виталию Харисову</a>, <a href="http://www.aether.ru/">Александру Шабуневичу</a>, <a href="http://makishvili.ya.ru/">Вадиму Макишвили</a>, <a href="http://mourner.livejournal.com/">Владимиру Агафонкину</a>.
<h3>Все советы</h3>
<ul>
<li><a href="http://rmcreative.ru/blog/post/neskolko-sovetov-verstalschikam">Александр RMcreative Макаров</a></li>
<li><a href="http://www.amazedev.com/5-sovetov-verstalshhiku/">Павел Коноплицкий</a></li>
<li><a href="http://habrahabr.ru/blog/webdev/43163.html">Владимир Mourner Агафонкин</a></li>
<li><a href="http://harisov.livejournal.com/105323.html">Виталий Харисов</a></li></li>
<li><a href="http://seleckis.lv/journal/css/5-sovetov-verstalschiku">Никита Селецкий</a></li>
<li><a href="http://uggallery.audiopeace.ru/2008/05/19/5-advices">Александр Исаков</a></li>
<li><a href="http://www.alexilin.ru/5-sovetov-po-html-i-css/">Алекс Iline</a></li>
<li><a href="http://www.aether.ru/blog/2008/06/04/5-advices">Александр Шабуневич</a></li>
<li><a href="http://blog.sribna.com/5-sovetov-verstalschiku.htm">Юрий Дроздов</a></li>
<li><a href="http://www.webmakerslounge.com/news/work-advices/">The Webmakers Lounge</a></li>
<li><a href="http://engelside.net/5-for-coder/">Engelside</a></li>
<li><a href="http://tanalin.com/blog/2008/05/xhtml-css-coding-tips-n-tricks/">Марат Таналин</a></li>
<li><a href="http://pepelsbey.net/2008/05/soviet-country/">Вадим Макеев</a></li>
<li><a href="http://cssing.org.ua/2008/05/21/5-things-to-remembe/">Юрий Артюх</a></li>
<li><a href="http://lusever.livejournal.com/21502.html">Павел Корнилов</a></li>
<li><a href="http://kizu.ru/webdev/five-tips/">kizu.ru</a></li>
</ul>
