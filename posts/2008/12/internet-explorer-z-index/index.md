---
title: "Internet Explorer и z-index"
date: "2008-12-07"
humanDate: "07 Dec, 2008"
permalink: "2008/12/07/internet-explorer-z-index/"
tags: 
  - "xhtmlcss"
  - "useful"
comments: 
  -  author: "nbaksalyar"
     id: "14656"
     url: ""
     date: "2009-07-22 17:16:18"
     humandate: "22 Jul, 2009"
     content: | 
       Огромное спасибо!
       После получасовых мучений с IE наконец-то помогло :)

     email: "n.baksalyar@yandex.ru"

  -  author: "akella"
     id: "14404"
     url: "http://cssing.org.ua"
     date: "2009-04-26 00:10:18"
     humandate: "26 Apr, 2009"
     content: | 
       Ну убрать relative для .entry не значит отказаться от него совсем, просто нужно попробовать применить его к другому элементу, чему-то внутри .entry, чтобы обойти баг в ИЕ.

     email: "akella.a@gmail.com"

  -  author: "Wincert"
     id: "14403"
     url: "http://W-blog.ru"
     date: "2009-04-25 18:30:43"
     humandate: "25 Apr, 2009"
     content: | 
       Столкнулся со второй проблемой...
       
       &gt;решение?
       &gt;Убрать position:relative для .entry
       
       С таким же успехом можно было бы написать: "Уволиться с должности верстальщика" - тоже неплохое решение этой проблемы.
       В реальных ситуациях position:relative не появляется просто так, если он стоит значит он там очень нужен. Пол сайта придется теперь переверстывать (((

     email: "Wincert@yandex.ru"

  -  author: "цук"
     id: "14344"
     url: ""
     date: "2009-04-08 12:37:46"
     humandate: "08 Apr, 2009"
     content: | 
       Никто не думал менять z-index у главного родительского елемента на 1000 к примеру при событии вызывающим попап (js естественно)?это решит ваши проблемы. И даже в том случае если у идущих подряд блоков индексы отличаются задайте их в диапазоне от 0 до 999.Этого диапазона вам за глаза хватит и попап всегда будет поверх.
       
       ЗЫ на возгласи типо "js может быть отключен в браузере" я отвечу: "У кого в браузере отключен javascript тому и попапы не нужны.

     email: "admin@wer.ru"

  -  author: "Анатлий"
     id: "14323"
     url: ""
     date: "2009-04-02 14:14:48"
     humandate: "02 Apr, 2009"
     content: | 
       Спасибо ОГРОМЕННОЕ!

     email: "sh_toly@mail.ru"

  -  author: "zmey"
     id: "14252"
     url: ""
     date: "2009-03-09 16:41:21"
     humandate: "09 Mar, 2009"
     content: | 
       спасибо за разъяснения

     email: "zmey1@rambler.ru"

  -  author: "Dimox"
     id: "13776"
     url: "http://dimox.name"
     date: "2008-12-07 13:37:07"
     humandate: "07 Dec, 2008"
     content: | 
       Очень мешает данное поведение IE, когда, бывает, хочется хитро извернуться в верстке. В результате приходится перемещать некоторые элементы кода в другое место.
       
       P.S. Юра, что стало со шрифтом на блоге? Шрифт стал мелким и пропало сглаживание.

     email: "dimox.name@mail.ru"

  -  author: "Юрко"
     id: "13775"
     url: ""
     date: "2008-12-07 12:41:29"
     humandate: "07 Dec, 2008"
     content: | 
       Ваш дiзайн — отстой!

     email: "zzz@xxx.yyy"

  -  author: "Genn"
     id: "13774"
     url: "http://genn.org/"
     date: "2008-12-07 12:35:48"
     humandate: "07 Dec, 2008"
     content: | 
       Никто никогда не обращает внимания на Гитлера.

     email: "soap@genn.org"

  -  author: "Евгений"
     id: "13778"
     url: "http://e-ivanov.com/"
     date: "2008-12-07 15:15:24"
     humandate: "07 Dec, 2008"
     content: | 
       абсолютные блоки для осла нужно перемещать в конец body.
       
       то есть, когда popup включаем, то перед этим делаем так
       
       $('.popup').insertBefore($(body));

     email: "eugene.ivanov@gmail.com"

  -  author: "angizij"
     id: "13779"
     url: "http://angizij.livejournal.com"
     date: "2008-12-07 15:15:34"
     humandate: "07 Dec, 2008"
     content: | 
       Не обращайте внимания на Гитлера.
       
       это из 3-х Tt Crowd ? )

     email: "angizij@ukr.net"

  -  author: "Spirit"
     id: "13780"
     url: ""
     date: "2008-12-07 15:20:15"
     humandate: "07 Dec, 2008"
     content: | 
       У меня самая распространенная проблема с z-index'ом - это выпадающие меню и какой-то absolute-ный или relative-ный контент. Лечилось выставлением z-index:1 для родителей выпадающего элемента по-очереди.

     email: "sp1r1t.vip@gmail.com"

  -  author: "jahson"
     id: "13781"
     url: ""
     date: "2008-12-07 17:34:39"
     humandate: "07 Dec, 2008"
     content: | 
       Всё дело в волшебных контекстах стэков :) У ИА с ними особое отношение.

     email: "jjahson@gmail.com"

  -  author: "pepelsbey"
     id: "13782"
     url: "http://pepelsbey.net"
     date: "2008-12-07 19:47:07"
     humandate: "07 Dec, 2008"
     content: | 
       Вот матерем клянусь — видел решение этой проблемы. Попробую применить гипноз и вспомнить…

     email: "pepelsbey@gmail.com"

  -  author: "pepelsbey"
     id: "13783"
     url: "http://pepelsbey.net"
     date: "2008-12-07 19:48:59"
     humandate: "07 Dec, 2008"
     content: | 
       Нашёл! Да здравствует делишез — <a href="http://aplus.rs/lab/z-pos/" rel="nofollow">Effect of z-index value to positioned elements</a>

     email: "pepelsbey@gmail.com"

  -  author: "akella"
     id: "13784"
     url: "http://cssing.org.ua"
     date: "2008-12-07 21:51:20"
     humandate: "07 Dec, 2008"
     content: | 
       Да, но его способ это задать для блоков-родителей z-index =(. Это обычно невозможно когда у нас список новостей, я ж как раз этот способ и написал (#2)
       
       @Dimox, боюсь что ты установил себе на винду шрифт Myriad. Ничего не могу поделать с ее пахабным сглаживанием к сожалению =( 
       
       IT Crowd хорош ;)

     email: "akella.a@gmail.com"

  -  author: "pepelsbey"
     id: "13785"
     url: "http://pepelsbey.net"
     date: "2008-12-07 22:06:17"
     humandate: "07 Dec, 2008"
     content: | 
       @akella: ну, почему — если мы правим баги для IE, то вполне можно использовать одноразовый expression, который расставит z-index'ы по списку.

     email: "pepelsbey@gmail.com"

  -  author: "akella"
     id: "13786"
     url: "http://cssing.org.ua"
     date: "2008-12-07 22:16:47"
     humandate: "07 Dec, 2008"
     content: | 
       И правда, забыл о нашем колдовстве :)
       
       Я, правда, решил по-другому, ставил position:relative блоку только при :hover. Таким образом его "деть" как и он сам был "на высоте" по сравнению с остальными без relative.

     email: "akella.a@gmail.com"

  -  author: "Genn"
     id: "13787"
     url: "http://genn.org/"
     date: "2008-12-07 22:32:12"
     humandate: "07 Dec, 2008"
     content: | 
       angizij, Вы будете удивлены, но чувство юмора есть не только у британских сценаристов.

     email: "soap@genn.org"

  -  author: "jahson"
     id: "13789"
     url: ""
     date: "2008-12-08 11:10:20"
     humandate: "08 Dec, 2008"
     content: | 
       Как это ни банально, но 
       http://css-discuss.incutio.com/?page=OverlappingAndZIndex
       И там всё есть )

     email: "jjahson@gmail.com"

  -  author: "akella"
     id: "13790"
     url: "http://cssing.org.ua"
     date: "2008-12-08 11:24:17"
     humandate: "08 Dec, 2008"
     content: | 
       Спасибо! Добавил в пост =)

     email: "akella.a@gmail.com"

  -  author: "SelenIT"
     id: "13791"
     url: ""
     date: "2008-12-08 12:17:04"
     humandate: "08 Dec, 2008"
     content: | 
       Спасибо! Буквально вчера пытался сам разобраться в спеке, кто из браузеров прав (причем мое имхо склонялось в пользу старых эксплореров). А тут по ссылкам в три клика нашлось доходчивое <a href="http://weblogs.mozillazine.org/hyatt/archives/2004_09.html#006469" rel="nofollow">объяснение</a>, почему правы современные браузеры, а IE6-7 заблуждаются :).
       
       Кстати, в самом стандартном режиме IE8 c z-index'ами уже тоже все в порядке. Хотя своих приколов с позиционированием пока тоже хватает, надеюсь, к релизу исправят...

     email: "selenit@mail.by"

  -  author: "xaOz"
     id: "13800"
     url: "http://xaoz.info"
     date: "2008-12-09 21:05:13"
     humandate: "09 Dec, 2008"
     content: | 
       Гитлер форева. Тьфу блин в смысле прикольно, но больше Гитлера не надо ).
       
       Шрифт в Висте ужасен полностью согласен - муть какая-то :(

     email: "xaoz@xaoz.info"

  -  author: "Snowcore"
     id: "13806"
     url: "http://snowcore.net"
     date: "2008-12-10 19:04:12"
     humandate: "10 Dec, 2008"
     content: | 
       скажите, а z-index одинаково ведет себя в IE6 и IE7 ?

     email: "snowcore.net@gmail.com"

  -  author: "Givi"
     id: "13837"
     url: ""
     date: "2008-12-18 00:50:17"
     humandate: "18 Dec, 2008"
     content: | 
       Свой вариант предложу: обрамляем все новости (новостные блоки) в общий блок, в котором делаем дочерний блок-попап с зет-индексом 1. Его позиционируем относительно родителя (общего блока), и проблем нема :)

     email: "strutik-givi@bigmir.net"

  -  author: "akella"
     id: "13808"
     url: "http://cssing.org.ua"
     date: "2008-12-11 02:28:15"
     humandate: "11 Dec, 2008"
     content: | 
       Да, в целом одинаково, и этот глюк тоже у них общий

     email: "akella.a@gmail.com"

  -  author: "cssing :: Архив :: CSSing 2008"
     id: "13902"
     url: "http://cssing.org.ua/2008/12/30/cssing-2008/"
     date: "2008-12-30 17:47:49"
     humandate: "30 Dec, 2008"
     content: | 
       [...] Internet Explorer и z-index &#8212; описание одного распространенного и вредного бага в ИЕ [...]

     email: ""

  -  author: "AMBA"
     id: "13905"
     url: "http://go.co.ua"
     date: "2009-01-01 13:21:39"
     humandate: "01 Jan, 2009"
     content: | 
       &gt;Задавать разные z-index для .entry. В случае новостей это невозможно, 
       
       Не совсем понимаю этот вывод, если новости генерятся, значит им автоматом можно и разные z-index сгенерить, по id или просто по итерациям цикла (с рассчётом чтобы максимально возможный не был больше чем используется где-то ещё на странице, если используется).

     email: "web@amba.net.ua"

  -  author: "akella"
     id: "13906"
     url: "http://cssing.org.ua"
     date: "2009-01-01 14:18:04"
     humandate: "01 Jan, 2009"
     content: | 
       Совершенно верно, можно задать разные. Но только в темплейтах этого не получится сделать =( да и лишние телодвижения, не очень красивое решение будет

     email: "akella.a@gmail.com"

  -  author: "AMBA"
     id: "13907"
     url: "http://go.co.ua"
     date: "2009-01-01 15:45:29"
     humandate: "01 Jan, 2009"
     content: | 
       1. ёпть, не ввёл 4 и пост потерялся, плохо. Надо поле подтверждения вынести ближе к кнопке "Отправить", и как-то выделить.
       2. страница с "Дважды два 4, нужно было ввести цифру 4 в поле." без указания кодировки, а не у всех по умолчанию включен утф.
       Отпало желание по второму разу писать то же, но попробую.
       
       Я давно смирился что практические и быстрые решения - не самые красивые и правильные с точки зрения каких-то стандартов "правильной" вёрстки.
       Держать оформление и вёрстку исключительно в шаблонах и цсс это скорее идеал, к нему можно стремится, но зачастую думаешь лишь о том чтобы всё работало, а не о том что завтра прийдётся менять дизайн и при этом возникнут лишние трудности. Помоему это зависит от ситуации, времени, верстает и порграмит один человек или разные, применяемых инструментов и решений, привычек и т.п. Хотя возможно я не дорос до того "уровня" когда всё верстается быстро, кроссбраузерно, идеально по всем стандартам, легко к изменению и красиво прои просмотре кода.
       
       P.S. &gt;в темплейтах этого не получится сделать =( 
       Это тоже не аксиома, смотря кто на чём темплейты строит, думаю не проблема передать в темплейт из модуля новости некое сгенерированное число, а в темплейте его использовать. Хотя лично я не совсем понимаю смысл такого |модуль выдающий данные в цикле|, тогда все данные получатся в одном блоке, или же сам шаблон надо будет прогонять через цикл n-раз, но зачем...

     email: "web@amba.net.ua"

  -  author: "AMBA"
     id: "13908"
     url: "http://go.co.ua"
     date: "2009-01-01 15:49:45"
     humandate: "01 Jan, 2009"
     content: | 
       Эмм, вырезаются теги, я имел ввиду [див style="z-index:x;"] |модуль выдающий данные в цикле|[/див]

     email: "web@amba.net.ua"

  -  author: "Сергей Прокопович"
     id: "13942"
     url: "http://seonews.ru"
     date: "2009-01-14 10:19:52"
     humandate: "14 Jan, 2009"
     content: | 
       &gt;Какие блоки дальше в коде, те и отобразятся поверх.
       
       А существуют ли какие-нибудь способы указания порядка расположения одного блока над другим? 
       У меня на блоге самописный движок, так вот там можно задавать параметры отображения для каждого блока в числовом значении. Оформляется это также через CSS.
       
       И еще: сейчас многие пробуют новую версию IE для вебмастеров. Там есть какие-то различия в отображении по сравнению с перечисленными релизами эксплорера?

     email: "sergey2009@ya.ru"

  -  author: "akella"
     id: "14028"
     url: "http://cssing.org.ua"
     date: "2009-02-02 15:15:00"
     humandate: "02 Feb, 2009"
     content: | 
       Обычно эту проблему (с оверлеем) решают отображением <a href="http://www.hedgerwow.com/360/bugs/activex-listbox/demo.php" rel="nofollow">ифрейма</a> с фильтром поверх селектов, он их "покрывает", а его прячут в СС, или меняют его ширину как надо через ЖС. Когда дело касалось хинтов, я обычно корректировал их позиции чтобы они с селектом не пересекались. Ну и приятно помнить что <a href="http://blogs.msdn.com/ie/archive/2006/01/17/514076.aspx" rel="nofollow">в ИЕ7 это решили</a>, хоть это и не освобождает от ИЕ6 ответственности.
       
       Возможно в вашем частном случае можно придумать что-то хитрое? Есть ли пример?

     email: "akella.a@gmail.com"

  -  author: "Nikita"
     id: "14024"
     url: "http://seleckis.lv"
     date: "2009-02-02 12:28:32"
     humandate: "02 Feb, 2009"
     content: | 
       Спасибо за пост. А теперь расскажите как расположить абсолютно-позиционируемый элемент поверх элементов форм? В IE6 всякие селекты вылезают на самый верхний уровень. Единственное решение нашел, тупо visibility:hidden скриптом прописывать, ну это только в том случае если используется что-то вроде lightbox/thickbox.

     email: "nikita@seleckis.lv"

  -  author: "akella"
     id: "14063"
     url: "http://cssing.org.ua"
     date: "2009-02-04 13:03:33"
     humandate: "04 Feb, 2009"
     content: | 
       Ну вот эти всякие лайтбоксы просто растягивают ифрейм в ИЕ6 и все.
       А что такого страшного в ифрейме? он ведь появится только для одного браузера? Ну сожрет он ему памяти, но и убирание всех селектов тоже откушает =)
       Но вариант со скрытием селектов на всей странице тоже отличный. 
       Просто как видно из блога разработчиков, сделать больше мало что можно. Все остальные хаки будут еще более грязные =)

     email: "akella.a@gmail.com"

  -  author: "Nikita"
     id: "14062"
     url: "http://seleckis.lv"
     date: "2009-02-04 12:24:08"
     humandate: "04 Feb, 2009"
     content: | 
       Ну как, если есть веб-сайт с контролами типа select (например last.fm, там сверху есть выбор раздела для поиска). При клике на сылку (например «Войти») появляется div развернутый на всё окно (сделаный примерно так же как lightbox), который затемняет всё содержимое веб-страницы. По центру затемненного фона появляетя форма входа, а сверху на этом же темном фоне вылезает упомянутый select.
       
       Насчёт iframe — не мой вариант. Терпеть его не могу. Лучше jQuery уберет контролы с глаз долой, а потом вернёт при закрытии попапа.
       
       Кстати, может лучше «поиск сбежавшего бота» поближе к кнопке «Отправить» поместить? А то замечаю это поле в последний момент :)

     email: "nikita@seleckis.lv"

  -  author: "Newone"
     id: "14161"
     url: ""
     date: "2009-02-18 13:02:57"
     humandate: "18 Feb, 2009"
     content: | 
       Эта проблема не только IE, я сталкивался с подобным и в других браузерах. для себя зарекся давать z-index абсолютным элементам которые меряются им с относительными. оборачиваю абсолютный в относительный и на него уже z-index.

     email: "m_konnov@list.ru"

  -  author: "Shady"
     id: "18660"
     url: ""
     date: "2010-05-20 01:19:31"
     humandate: "20 May, 2010"
     content: | 
       Сначала всегда считала, что обходить подобные вещи можно только располагая выпадающее меню в самом низу страницы и position:absolute подгонять в нужное место. Когда надо, чтобы весь сайт центрировался это заставляло перепланировать полностью структуру сайта и делать чуть ли не весь сайт на абсолютах (left:50% ... left:-300px ...) и в этом полно своих минусов.
       И как-то случайно вспомнила про z-index ... и все бы ничего, но в IE6-7 не работает. И только наткнувшись на вашу статью (и это время сказать спасибо за нее) вспомнила что даже в htmlbook читала об relative или absolute для z-index но успешно об этом позабыла.

     email: "shady@yunack.com"

  -  author: "DDSSDD"
     id: "18716"
     url: ""
     date: "2010-06-24 18:25:43"
     humandate: "24 Jun, 2010"
     content: | 
       Долго искал решение проблемы с Z-idex и IE6. Но решилось все просто - http://tjkdesign.com/articles/z-index/teach_yourself_how_elements_stack.asp 
       Подобрал, открыв эту ссылку в IE6 позиционирование и значение Z-idex для двух верхних блоков. Оказывается нужно было задать для нижнего блока значение Z-Index: - 1; позиционирование realativ , у верхнего static и положительный Z-Index и IE все прекрасно понял. Дочернее меню стало отображаться над нижним блоком.

     email: "DDSSDD@i.ua"

  -  author: "Роман"
     id: "18764"
     url: "http://webcocktail.ru"
     date: "2010-08-12 16:38:10"
     humandate: "12 Aug, 2010"
     content: | 
       Вот тут объясняется проблема: http://www.webcocktail.ru/coding/z-index-position-bug-in-internet-explorer/
       У родительских блоков, содержащих в себе блоки с абсолютным позиционированием, также должен быть указан z-index. Именно он и влияет в IE на то, какой блок будет находится "выше".

     email: "roman.cssdesigner@gmail.com"

  -  author: "Константин"
     id: "21580"
     url: "http://www.sev-info.net"
     date: "2011-09-11 14:42:28"
     humandate: "11 Sep, 2011"
     content: | 
       Спасибо! 
       Толково и доходчиво. 
       Проблема решена

     email: "admin@sev-info.net"

  -  author: "Дмитрий"
     id: "21032"
     url: "http://madex-design.ru"
     date: "2011-09-01 14:21:56"
     humandate: "01 Sep, 2011"
     content: | 
       Блин, спасибо!

     email: "madex@yandex.ru"

  -  author: "Владимир"
     id: "24087"
     url: "http://ww.qdinov.ru"
     date: "2011-10-24 13:23:12"
     humandate: "24 Oct, 2011"
     content: | 
       Очень интересный пост, и, главное, нравится Ваш подход с юмором. Но к сожалению мою проблему с z-index в IE8 она не решила...

     email: "mail@qdinov.ru"

  -  author: "Юля"
     id: "75195"
     url: ""
     date: "2012-08-28 12:27:21"
     humandate: "28 Aug, 2012"
     content: | 
       такой эффект я встречаю и в современных браузерах, фбсолют ложится под релатив..

     email: "sk8_2er@mail.ru"

  -  author: "ivanko"
     id: "57332"
     url: ""
     date: "2012-05-21 13:23:30"
     humandate: "21 May, 2012"
     content: | 
       111

     email: "ivanko@taran.com"

  -  author: "ivanko"
     id: "57333"
     url: "http://'"
     date: "2012-05-21 13:23:53"
     humandate: "21 May, 2012"
     content: | 
       1

     email: "ivanko@taran.com"

  -  author: "Михаил"
     id: "43104"
     url: ""
     date: "2012-03-07 15:50:17"
     humandate: "07 Mar, 2012"
     content: | 
       Спасибо! про z-index для родителя сам бы никогда не догадался

     email: "m@korotaev.ru"

  -  author: "Алексей"
     id: "156919"
     url: ""
     date: "2013-07-21 00:44:49"
     humandate: "21 Jul, 2013"
     content: | 
       спасибо! помогло с z-index "родителей" для 8 ИЕ (другие уже не волнуют)

     email: "alex.veider@gmail.com"

layout: "layouts/post.njk"
excerpt: "ИЕ воспринимает z-index не совсем так, как все остальные браузеры. Это поведение настолько часто встречается в моей жизни, что я решил о нём написать целый пост."
---

ИЕ воспринимает z-index не совсем так, как все остальные браузеры. Это поведение настолько часто встречается в моей жизни, что я решил о нём написать целый пост.<!--more-->
Меня часто просят поправить ошибки в верстке. Так вот эта &#8212; входит в топ-5.
<h3>z-index работает?</h3>
Да, совершенно точно работает. Берем два блока, с position:absolute (для работы z-index нужен либо <code>relative</code> либо <code>absolute</code>)
Задаем им обоим что-то такое:
<ol class="code">
<li>#block1, #block2{</li>
<li class="tab">position:absolute</li>
<li>}</li>
<li>#block1{z-index:10}</li>
<li>#block2{z-index:20}</li>
</ol>
<p class="img"><img src="http://cssing.org.ua/pic/iezindex/zigindex.png" width="406" height="346" alt="иллюстрация z-index" /><span>На самом деле, мне просто больше нравятся зеленые блоки. <br />Не обращайте внимания на Гитлера.</span></p>
Блок с б<em>о</em>льшим z-index отобразится поверх блока с меньшим z-index. Все как бы работает. И в IE в том числе.
<h3>работает, но...</h3>
Классическая обстановка для &laquo;проблемы в вёрстке&raquo;.

В коде идут подряд два блока с <code>position:relative</code>. Например, два блока новости, или блоки вроде header и content. В relative ничего необычного нет, может добавили для absolute блоков внутри, или <a href="http://cssing.org.ua/2005/11/11/ie-magic/">для хаков</a>.
Как-то так:
<ol class="code">
<li>&lt;div class=&quot;entry&quot;&gt;&lt;/div&gt;</li>
<li>&lt;div class=&quot;entry&quot;&gt;&lt;/div&gt;</li>
</ol>
И теперь, например, в одном из них появляется всплывающее окошко, или попап, или выпадающее меню:
<ol class="code">
<li>&lt;div class=&quot;entry&quot;&gt;</li>
<li class="tab">&lt;div class=&quot;popup&quot;&gt;Попап&lt;/div&gt;</li>
<li>&lt;/div&gt;</li>
<li>&lt;div class=&quot;entry&quot;&gt;&lt;/div&gt;</li>
</ol>
И такой вот дизайн:
<p class="img"><img src="http://cssing.org.ua/pic/iezindex/right.png" width="351" height="167" alt="поведение всех броузеров кроме ИЕ" /><span>Попап должен находиться в блоке 1</span></p>
Будь вы мной, вы написали бы такой CSS:
<ol class="code">
<li>.entry{</li>
<li class="tab">position:relative</li>
<li class="tab">}</li>
<li>.popup{</li>
<li class="tab">position:absolute;</li>
<li class="tab">z-index:10;</li>
<li class="tab">top:10px;left:100px;</li>
<li class="tab">}</li>
</ol>
Если добавить цвета и размеры, <a href="http://cssing.org.ua/examples/iezindex/">все отобразится</a> и правда так, как в дизайне.
Но, разумеется, не в ИЕ.

Там это будет выглядеть так:
<p class="img"><img src="http://cssing.org.ua/pic/iezindex/wrong.png" width="339" height="166" alt="так выглядит в ИЕ" /><span>Попап или выпадающее меню скроется за следующие блоки</span></p>
Я это понимаю так: ИЕ сравнивает не только z-index блоков, но и z-index их родителей. Причем родительский важнее. В моем примере роль &laquo;родительского z-index&raquo; исполняет просто последовательность блоков в коде. Какие блоки дальше в коде, те и отобразятся поверх.


Я сделал <a href="http://cssing.org.ua/examples/iezindex/">специальный пример</a>, смайлик из acid-теста будет улыбаться всем браузерам кроме ИЕ. (его улыбка зависит от этого вот поведения с relative блоками)
<h3>решение?</h3>
<ol>
<li>Убрать position:relative для .entry</li>
<li>Задавать разные z-index для .entry. В случае новостей это невозможно, они ведь генерируются симметрично. Однако когда у нас header и content, вполне подходит.</li>
</ol>
Может быть есть еще?
<h3>В конце</h3>
Мне не хочется называть это багом, поскольку для него требуется куча обстоятельств, скорее всего не описанных w3c. (или описанных?)
Поведение имеет место в IE5-7. <del datetime="2008-12-08T09:13:21+00:00">И, наверное, 8.</del>
Как всегда буду рад вашему опыту и мыслям по этому поводу. 
Статьи на тему этого поведения:
<ul>
<li><a href="http://css-discuss.incutio.com/?page=OverlappingAndZIndex">Stacking context</a></li>
<li><a href="http://aplus.rs/lab/z-pos/" rel="nofollow">Effect of z-index value to positioned elements</a></li>
</ul>
