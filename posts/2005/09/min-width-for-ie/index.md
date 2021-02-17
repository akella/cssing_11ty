---
title: "min-width для IE"
date: "2005-09-02"
humanDate: "02 Sep, 2005"
permalink: "2005/09/02/min-width-for-ie/"
tags: 
  - "xhtmlcss"
  - "useful"
comments: 
  -  author: "edgy"
     id: "2249"
     url: "http://blog.edgy.ru/"
     date: "2005-09-05 10:50:22"
     humandate: "05 Sep, 2005"
     content: | 
       Попробуйте сделать в IE border шире 960 пикселей.
       Весело, ага.

     email: "i@edgy.ru"

  -  author: "akella"
     id: "2250"
     url: "http://cssing.iatp.org.ua"
     date: "2005-09-05 10:55:25"
     humandate: "05 Sep, 2005"
     content: | 
       А что там такое страшное происходит? Интересно ж...
       
       Ну а когда нам понадобится min-width:960px думаю ИЕ уже будет это поддерживать...

     email: "akella.a@gmail.com"

  -  author: "kost"
     id: "2325"
     url: "http://reg.kost.ru"
     date: "2005-09-23 14:39:09"
     humandate: "23 Sep, 2005"
     content: | 
       Понадобилось как-то для ширины больше 960px. А то некоторые «дезайниры» считают, что людей с браузером открытым меньше чем в 1024&#215;768 уже нет.
       
       При min-width &gt; 960 px в IE6 контент сползает влево на ширину, равную min-width-960. Причем в IE5 этого не наблюдается (если мне не изменяет память).
       
       На сайте http://www.cssplay.co.uk/ когда-то были комментарии, я спросил, ответили, что в transparent варианте (http://www.cssplay.co.uk/boxes/min-widthSn.html) с этим все нормально.

     email: "kost@kost.ru"

  -  author: "gam"
     id: "2415"
     url: ""
     date: "2005-10-10 11:32:34"
     humandate: "10 Oct, 2005"
     content: | 
       Ну и 4-й самый тривиальный способ, но может и не всем интересный - вставка 1-нопиксельного прозрачного gif'а с нужной шириной. ;)

     email: "design@greenkey.ru"

  -  author: "cssing :: Архив   :: cssing 2005"
     id: "2681"
     url: "http://cssing.org.ua/2005/12/27/cssing-highlights-2005/"
     date: "2005-12-27 14:59:24"
     humandate: "27 Dec, 2005"
     content: | 
       [...] временем - алистапартовская байка про time management. Бородатая но все равно актуальная. min-width для IE - обзор 3 способов как это лучше делать. 	Прелоад через CSS - способы подзагр [...]

     email: ""

  -  author: "grlm"
     id: "2793"
     url: "http://blog.grlm.ru"
     date: "2006-02-21 09:00:32"
     humandate: "21 Feb, 2006"
     content: | 
       &lt;----&gt; перед доктайпом и способ #1 рулят :)

     email: "default@bk.ru"

  -  author: "akella"
     id: "2801"
     url: "http://cssing.org.ua"
     date: "2006-02-26 16:11:28"
     humandate: "26 Feb, 2006"
     content: | 
       А еще рулит изменения значения 770 на 771 например. То есть стоит поиграться +- 1 пиксел в exression - почти наверняка помогает

     email: "akella.a@gmail.com"

  -  author: "эдик"
     id: "2917"
     url: ""
     date: "2006-03-30 11:11:27"
     humandate: "30 Mar, 2006"
     content: | 
       А как с доктайпом поиграться?Вот пытаюсь сделать max-height для блока,даже Опера(!)не понимает.(правда у меня маргины по десять процентов стоят-ну думаю наврядли они во всем виноваты).

     email: "zoulou@hotbox.ru"

  -  author: "akella"
     id: "2919"
     url: "http://cssing.org.ua"
     date: "2006-03-30 15:28:41"
     humandate: "30 Mar, 2006"
     content: | 
       "Поиграться" - я имел ввиду попробовать менять разные доктайпы.
       
       А всего кода Вашего я не вижу - поэтому вряд ли могу помочь более конкретно. Смена доктайпа предназначается только для ИЕ и того джаваскриптового решения...

     email: "akella.a@gmail.com"

  -  author: "wil"
     id: "2947"
     url: ""
     date: "2006-04-14 11:41:13"
     humandate: "14 Apr, 2006"
     content: | 
       как все сложно....ыыыы

     email: "asd@mail.ru"

  -  author: "Script"
     id: "4630"
     url: "http://www.free-lance.ru/users/script"
     date: "2006-08-28 19:14:53"
     humandate: "28 Aug, 2006"
     content: | 
       По поводу 3-го поста (насчёт min-width &gt; 960 px):
       Тоже столкнулся с такой проблемой при использовании 2-го способа, описанного в данной статье, и решил её простым добавлением _margin-left: "min-width-960px" в body, и всё стало зашибись! =)
       т.е. получилось такое:
       body {
        min-width: 997px;
        margin: 0;
        _margin-left: 37px;
        padding: 0;
       }
       
       P.S.: Автору - ОГРОМНЫЙ РЕСПЕКТ!!! Меня эта проблема давно доставала.

     email: "webber@mail.ru"

  -  author: "faxenoff"
     id: "4619"
     url: "http://www.artin.ru"
     date: "2006-08-27 23:50:52"
     humandate: "27 Aug, 2006"
     content: | 
       Самое лучшее JS-решение
       http://toserveman.kalebwalton.com/articles/2006/08/02/ie-min-width-css-workaround

     email: "faxenoff@gmail.com"

  -  author: "akella"
     id: "8343"
     url: "http://cssing.org.ua"
     date: "2007-02-16 23:29:36"
     humandate: "16 Feb, 2007"
     content: | 
       Лучше просто дай ссылку на рабочий пример - видать там было упоминание тага, а у меня разрешен ХТМЛ каментах.

     email: "akella.a@gmail.com"

  -  author: "[e]Bu$ter"
     id: "8362"
     url: "http://eppz.net"
     date: "2007-02-17 17:13:48"
     humandate: "17 Feb, 2007"
     content: | 
       Там есть знак "больше либо равно" и "меньше либо равно" — это он видимо «смущает» движок...
       Удалите все мои предыдущие посты, пользы от них в таком виде всё равно никакой (они же одинаковые все). Ссылки на рабочий пример тоже пока нет – в разработке.
       
       Ладно, последняя попытка (если получится тоже самое что и в предыдущих постах, удалите и этот):
       [code]
       function bodySize(){
        sObj = document.getElementsByTagName("body")[0].style;
        if (document.documentElement.clientWidth&lt;=760) {
        sObj.width = "600px";
        } else if (document.documentElement.clientWidth&gt;=1100) {
        sObj.width = "900px";
        } else {
        sObj.width = "80%";
        }
       }
       
       if(navigator.appName == "Microsoft Internet Explorer") {
        onresize = bodySize;
        onload = bodySize;
       }
       [/code]
       
       Смысл такой: <strong>body</strong> всегда занимает 80% от ширины окна в диапазоне ширины окна от 760px и до 1100px. Как только ширина окна выходит из заданного диапазона, растягивание (или сжатие) <strong>body</strong> в IE прекращается. Проще говоря, сей костыль реализует подержку min-width и max-width в IE.

     email: "eBuster@mail.ru"

  -  author: "Cybersurfer"
     id: "8630"
     url: "http://paradox-studio.biz/"
     date: "2007-02-22 08:36:38"
     humandate: "22 Feb, 2007"
     content: | 
       Только что столкнулся с проблемой min-width &gt; 960 px, решение действительно работает по схеме "двух обертывающих дивов" просто если используется min-width&gt; 960 то из min-width вычитаем 960 и пишем получившуюся цифру в margin-left для body.
       Пример:
       * html body{
        margin: 0 0 0 40px;
       }
        /*для всех броузеров что понимают min-width */
        #min-width {
        min-width:1000px;
        }
        /* для IE */
        * html .minwidth {
        border-left:1000px solid #fff;/*min-width*/
        position:relative;
        float:left;
        z-index:1;
        }
        * html .container {
        margin-left:-1000px; /*-min-width*/
        position:relative;
        float:left;
        z-index:2;
        }
       все работает!

     email: "cyber5urfer@yandex.ru"

  -  author: "CTAJIKEP"
     id: "9847"
     url: ""
     date: "2007-03-21 07:19:21"
     humandate: "21 Mar, 2007"
     content: | 
       А не пробовали просто изменить немного так
       
       * html .container {
       margin-left:-960px; /*-min-width*/
       position:relative;
       float:left;
       z-index:2;
       }
       
       Зачем еще и body трогать? . :)

     email: "sia@r-soft.ru"

  -  author: "Magentoua"
     id: "18576"
     url: "http://magentoua.wordpress.com/"
     date: "2010-04-19 13:42:20"
     humandate: "19 Apr, 2010"
     content: | 
       39. Александр
       "Что означает запись * html в css?"
       - Це відсічка на Internet Explorer 6. Тобто стрічка яка починається з * html буде зрозуміла тільки IE6

     email: "magentoua@gmail.com"

  -  author: "askari"
     id: "18526"
     url: ""
     date: "2010-04-04 23:58:06"
     humandate: "04 Apr, 2010"
     content: | 
       март 2010-ого..нано технологии стремительно рвуться вперёд. max-width по прежнему не работает

     email: "ti_komaro@mail.ru"

  -  author: "Ilya"
     id: "14942"
     url: ""
     date: "2009-11-25 12:49:11"
     humandate: "25 Nov, 2009"
     content: | 
       На дворе конец 2009 года, в ходу ie8. за 4 года max-width так и не заработал.

     email: "qwerty468@ya.ru"

  -  author: "Евгений"
     id: "14620"
     url: "http://csbet.ru"
     date: "2009-07-10 08:56:46"
     humandate: "10 Jul, 2009"
     content: | 
       Мы знакомы всего несколько минут, но кажется, я люблю вас =))
       Спасибо за статью.
       Очень во время помогли.

     email: "hunterxp@mail.ru"

  -  author: "tolstyj"
     id: "10954"
     url: ""
     date: "2007-05-17 15:46:08"
     humandate: "17 May, 2007"
     content: | 
       выход в случае с шириной больше 960px:
       <pre>
       /*для всех броузеров что понимают min-width */
       #min-width {
        min-width:1000px; 
        }
       /* для IE */
       * html .minwidth {
        border-left:960px solid #fff;
        border-right:40px solid #fff;/*min-width-960*/
        position:relative; 
        float:left; 
        z-index:1;
        }
       * html .container {
        margin-left:-960px; /*-min-width*/
        margin-right:-40px; /*-(min-width-960)*/
        position:relative; 
        float:left; 
        z-index:2; 
        }
       </pre>

     email: "snake_@bk.ru"

  -  author: "nick"
     id: "11155"
     url: ""
     date: "2007-09-04 00:41:44"
     humandate: "04 Sep, 2007"
     content: | 
       помогло, спасибо..

     email: "nnrybakov@gmail.com"

  -  author: "SelenIT"
     id: "11451"
     url: ""
     date: "2007-12-12 04:48:05"
     humandate: "12 Dec, 2007"
     content: | 
       &gt; Смена доктайпа и еще пару примочек помогает. Например переход XHTML на HTML спасает.
       
       Не может спасать переход "XHTML на HTML" - хотя бы по той простой причине, что XHTMLя в IE просто не бывает). Спасает переход из Strict mode в Quirks mode (именно это, кстати, происходит в IE6 при вставке чего угодно перед доктайпом). А все потому, что в Quirks document.body является внешним контейнером, а в Strict он сам вложен в document.documentElement, от которого и нужно "плясать".
       
       "Играться" с доктайпами смысла не вижу - какой из них дает какой режим рендеринга, давно известно (http://hsivonen.iki.fi/doctype/), нужно просто выбрать наиболее подходящий по результату сообразно задаче.
       
       Простите за резкость, просто задрал уже этот миф про "волшебную букву X"...

     email: "selenit@mail.by"

  -  author: "akella"
     id: "11452"
     url: "http://cssing.org.ua"
     date: "2007-12-12 11:18:04"
     humandate: "12 Dec, 2007"
     content: | 
       XHTML настоящего в ИЕ нет, но смена XHTML доктайпа на HTML действительно иногда помогает, и это без quirks mode.
       
       Мифа нет, вы попробуйте просто =) Не знаю где вы тут миф этот нашли - я уже писал о том что такое настоящий XHTML - http://cssing.org.ua/2005/02/25/xhtml-worth-or-not/ почти 3 года назад )

     email: "seijuro@yandex.ru"

  -  author: "Wakh"
     id: "11643"
     url: "http://wakh.viart.ru"
     date: "2008-01-13 18:12:03"
     humandate: "13 Jan, 2008"
     content: | 
       использовал первый метод - ширина 995px
       http://avia2.mosaero.org/
       теперь возникла проблема с исчезновением картинок-бэков в ИЕ, если:
       1. сделать размер окна 800х600, а потом распахнуть (по Ф5 не лечится)
       2. сделать размер окна 1024х768 и выше (лечится если распахнуть (и обратно))

     email: "wakhw@viart.ru"

  -  author: "Wakh"
     id: "11646"
     url: "http://wakh.viart.ru"
     date: "2008-01-14 12:00:21"
     humandate: "14 Jan, 2008"
     content: | 
       прочитав http://xpoint.ru/forums/internet/html_css/css/thread/34023.xhtml
       помогло "зум:1" ура!

     email: "wakhw@viart.ru"

  -  author: "mrAdamoff"
     id: "12003"
     url: ""
     date: "2008-03-18 17:43:33"
     humandate: "18 Mar, 2008"
     content: | 
       спасибо, очень помогло.
       Для ширины более 960px использовал вариант <b>tolstyj</b>.
       Только в контейнере опечатка, второй марджин предназначается естественно для правой границы.

     email: "27august@mail.ru"

  -  author: "akella"
     id: "12005"
     url: "http://cssing.org.ua"
     date: "2008-03-19 02:54:35"
     humandate: "19 Mar, 2008"
     content: | 
       Спасибо! 
       Теперь все верно, подправил его комментарий

     email: "akella.a@gmail.com"

  -  author: "Webych"
     id: "12063"
     url: "http://www.webych.ru"
     date: "2008-03-31 23:02:03"
     humandate: "31 Mar, 2008"
     content: | 
       Почему вставка однопиксельного (в высоту) div'а или gif'а не помогает?

     email: "webych@gmail.com"

  -  author: "CSS XHTML &#8220;Шпаргалка на промокашке&#8221; &laquo; Студия AlterEgo. Блог"
     id: "12188"
     url: "http://alterego.biz.ua/blog/2008/04/06/css-xhtml-%d1%88%d0%bf%d0%b0%d1%80%d0%b3%d0%b0%d0%bb%d0%ba%d0%b0-%d0%bd%d0%b0-%d0%bf%d1%80%d0%be%d0%bc%d0%be%d0%ba%d0%b0%d1%88%d0%ba%d0%b5/"
     date: "2008-04-06 11:50:16"
     humandate: "06 Apr, 2008"
     content: | 
       [...] Учим ИЕ "плохому" — min-width, max-width * «min-width для IE» (cssing.org.ua/2005/09/02/..) * «max-width в Internet Explorer» (xhtml.ru/2005/06/11/max-w..) * «min-width for Internet [...]

     email: ""

  -  author: "Санча"
     id: "12333"
     url: "http://rs-creative.com"
     date: "2008-04-28 15:49:12"
     humandate: "28 Apr, 2008"
     content: | 
       не знаю что ставит в тупик IE, но я вместо строго неравенства, поставил &lt;=, и при этом глюк упорхнулв небытие. Во всяком случае на моём компе.
       
       Очень интересно знать от чего есть подвисание, и если подвисание не наблюдается у меня, возможно ли оно на машине пользователя.

     email: "alex@rs-creative.com"

  -  author: "Александр"
     id: "14460"
     url: ""
     date: "2009-05-28 09:57:39"
     humandate: "28 May, 2009"
     content: | 
       Что означает запись * html в css ?

     email: "i3bepb@e1.ru"

  -  author: "Фдучфтвук"
     id: "12605"
     url: ""
     date: "2008-06-07 17:02:05"
     humandate: "07 Jun, 2008"
     content: | 
       #all {
       text-align:center;
       min-width:1000px;
       width:expression(((document.compatMode &amp;&amp; document.compatMode=='CSS1Compat') ? document.documentElement.clientWidth : document.body.clientWidth) &lt; 1020 ? "1020px" : "auto");
       }
       У меня чтои ттакой скрипт в css все пашет все супер ) но это не валидно ) что подскажите по этому поводу. ПОнимаю конечно что всем плевать на валидацию цсс, но все же.

     email: "pipenyo@list.ru"

  -  author: "рус"
     id: "14402"
     url: ""
     date: "2009-04-25 18:25:00"
     humandate: "25 Apr, 2009"
     content: | 
       Юрий,
       в ИЕ6 твой пример тупо задает фиксированную ширину, так что можешь сам пойти ;)

     email: "rus@mail.ru"

  -  author: "Kor-Elf"
     id: "12696"
     url: "http://kor-elf.kz"
     date: "2008-06-24 09:27:51"
     humandate: "24 Jun, 2008"
     content: | 
       #site{min-width:1000px;}
       *html #site{
       -width:1000px;
       z-index:1;
       	height:0px;
       	margin:0px;
       	padding:0px;
       	background:transparent;
       	color:transparent;
       	}
       мне это помогло! и без скриптов!

     email: "Leonid@kor-elf.kz"

  -  author: "Jony"
     id: "12870"
     url: ""
     date: "2008-07-14 17:38:21"
     humandate: "14 Jul, 2008"
     content: | 
       я подобную задачу решил пустым гифом + overflow:scroll. вроде такого:
       
       &lt;img alt="" src="empty.gif" width="1024" height="0" style="overflow:scroll; margin:0px; padding:0px;"&gt;
       
       . как результат - в блоке содержащем этот гиф появляется скролбар после уменьшения ширины меньше 1024. да и вообще с overflow:scroll можно в этих целях эксперементировать. весьма просто и без инvalidности. хотя в ie из за этого могут возникнуть проблемы с отступами, но при желании они легко решаются.

     email: "ololo@mail.edu"

  -  author: "Семантическая верстка — советы и решения. Часть VIII. Минимальные и максимальные размеры"
     id: "13148"
     url: "http://flack.ru/2008/08/26/semantic-coding-howto-8/"
     date: "2008-08-26 14:33:08"
     humandate: "26 Aug, 2008"
     content: | 
       [...] min-width для IE [...]

     email: ""

  -  author: "Женя"
     id: "13375"
     url: ""
     date: "2008-10-11 02:14:15"
     humandate: "11 Oct, 2008"
     content: | 
       # #min-width {
       # width:50%;
       # min-width:400px;
       # }
       # /* для IE */
       # * html .minwidth {
       # border-left:400px solid #fff;/*min-width*/
       # position:relative;
       # float:left;
       # z-index:1;
       # }
       # * html .container {
       # margin-left:-400px; /*-min-width*/
       # position:relative;
       # float:left;
       # z-index:2;
       # }
       У меня вопрос по поводу второго метода. Я его использовал. Все супер. Но вот тоько фон моей рабочей зоны которая в .winwidth в ИЕ: белая. Я заменил цвет на тот который у меня на сайте, благо это просто замена цвета. но а если это уникальный цвет, т.е. постоянно меняющийся , который нужн будет отрезать одним пикселем и повторить по всей ширине? ТО белый цвет вмешается в мои планы?

     email: "jenyaz@mksat.net"

  -  author: "akella"
     id: "13380"
     url: "http://cssing.org.ua"
     date: "2008-10-11 22:24:00"
     humandate: "11 Oct, 2008"
     content: | 
       Совершенно верно, в методе проблемы когда нужен свой фон. Потому существует усложненный вариант - там 4 дива обертки, вот <a href="http://www.cssplay.co.uk/boxes/min-widthSn.html" rel="nofollow">тут второй пример</a>

     email: "akella.a@gmail.com"

  -  author: "Эмуляция min-width, max-width под IE6 | ZODIOS.net"
     id: "13534"
     url: "http://zodios.net/htmlcss/min-width-max-width-ie6.html"
     date: "2008-11-08 22:11:59"
     humandate: "08 Nov, 2008"
     content: | 
       [...] Источник материала [...]

     email: ""

  -  author: "min-width в Internet Explorer | HTML-CODER.ORG.RU"
     id: "13815"
     url: "http://html-coder.org.ru/web/min-width-%d0%b2-internet-explorer/"
     date: "2008-12-12 23:11:58"
     humandate: "12 Dec, 2008"
     content: | 
       [...] Вариант с JavaScript (да и еще много всего) можно подсмотреть на cssing.org.ua/2005/09/02/min-width-for-ie [...]

     email: ""

  -  author: "min-width в Internet Explorer | HTML-CODER.ORG.RU"
     id: "13927"
     url: "http://html-coder.org.ru/web/min-width-internet-explorer/"
     date: "2009-01-10 22:55:58"
     humandate: "10 Jan, 2009"
     content: | 
       [...] Вариант с JavaScript (и еще много всего) можно подсмотреть на cssing.org.ua/2005/09/02/min-width-for-ie [...]

     email: ""

  -  author: "Юрий"
     id: "14020"
     url: "http://vsape.info"
     date: "2009-01-31 06:08:39"
     humandate: "31 Jan, 2009"
     content: | 
       min-width:1000px;
       width:auto !important;
       width:1000px;
       
       И идите нахуй со своими костылями LOL

     email: "addurl@yandex-team.ru"

  -  author: "Олег"
     id: "18671"
     url: ""
     date: "2010-05-25 15:39:53"
     humandate: "25 May, 2010"
     content: | 
       # 17 мне помог, спс большое

     email: "jktugg@mail.ru"

  -  author: "min-width для IE | Искусство создания и продвижения сайтов"
     id: "18726"
     url: "http://www.fortress-design.com/layout/min-width-ie/"
     date: "2010-06-29 18:39:27"
     humandate: "29 Jun, 2010"
     content: | 
       [...] min-width для IE Теги:&nbsp;&nbsp;ie [...]

     email: ""

  -  author: "Олег"
     id: "18729"
     url: "http://savvateev.org"
     date: "2010-06-30 12:39:37"
     humandate: "30 Jun, 2010"
     content: | 
       Вот еще один способ <a href="http://savvateev.org/blog/20/" rel="nofollow">http://savvateev.org/blog/20/</a>

     email: "O.Savvateev@gmail.com"

  -  author: "Виталий Капля"
     id: "18762"
     url: "http://dropbydrop.org.ua/"
     date: "2010-08-11 12:52:40"
     humandate: "11 Aug, 2010"
     content: | 
       Спасибо, все отлично, вот только примеры куда-то сбежали =)

     email: "dropbydrop@ukr.net"

  -  author: "DeathBloom"
     id: "18932"
     url: ""
     date: "2010-11-05 15:18:09"
     humandate: "05 Nov, 2010"
     content: | 
       Немного оффтоп, но использованное словосочетания "такова селяви" - указывает на незнание автором перевода французского выражения "c'est la vie" и, как следствие, автор строит неправильные словосочетания с этой фразой.
       c'est la vie - "такова жизнь". В итоге получаем "такова такова жизнь" - глупость.
       Правильный вариант употребить просто "се ля ви". Или уже "такова la vie", но никак не то, что написал автор.

     email: "deathblooms@rambler.ru"

  -  author: "akella"
     id: "18933"
     url: "http://cssing.org.ua"
     date: "2010-11-05 15:21:46"
     humandate: "05 Nov, 2010"
     content: | 
       <blockquote>В итоге получаем “такова такова жизнь” - глупость.</blockquote>
       Exactly =)
       Спасибо я прекрасно знаю его значение, для того и использую этот тавталогичный каламбур. Я наивно полагал что значение слов "се ля ви" достаточно очевидно для всех, чтобы с ним можно было шутить :)

     email: "akella.a@gmail.com"

  -  author: "Елена"
     id: "21754"
     url: ""
     date: "2011-09-15 21:26:57"
     humandate: "15 Sep, 2011"
     content: | 
       Конец 2011 года)) Все еще с костылями)) Эту страницу нужно отправить в майкрософт)))

     email: "leftbox2005@yandex.ru"

  -  author: "Songo"
     id: "116966"
     url: "http://cssing.org.ua"
     date: "2013-01-01 21:34:37"
     humandate: "01 Jan, 2013"
     content: | 
       Начало 2013 года, исследуем Марс, покуда всё Ок :), а ie6 всё еще даёт о себе знать :( Интересно, Била икота не замучила?

     email: "asfds@mail.ru"

layout: "layouts/post.njk"
excerpt: "<del datetime=\"2005-09-23T15:56:39-03:00\">Два</del><strong>Три</strong> способа как это можно сделать в ИЕ...
"
---

<del datetime="2005-09-23T15:56:39-03:00">Два</del><strong>Три</strong> способа как это можно сделать в ИЕ...
<!--more-->
<h3>min-width по нормальному</h3>
Это очевидно, так <strong>должно</strong> быть, это должно работать:
<ol class="code">
<li>#min-width {</li>
<li class="tab">min-width:600px;</li>
<li>}</li>
</ol>
Но, как вы можете легко догадаться, работает везде, кроме чего? 
Правильно! Интернет Эксплорера! :)
<h3>Вступление</h3>
Здесь и дальше я буду укрощать(задавать минимальную ширину) блок <strong>#min-width</strong>.
<h3>Метод 1: JavaScript</h3>
Вот такой простенький кусок CSS (перемешанного с JS) решает проблему..
<ol class="code">
<li>#min-width {</li>
<li class="tab">min-width:800px;</li>
<li class="tab">width:expression(document.body.clientWidth < 770? "770px": "auto" );</li>
<li>}</li>
</ol>
Или так например:
<ol class="code">
<li>* html #min-width {</li>
<li class="tab">width:expression(document.body.clientWidth > 770? "100%" :"770px");</li>
<li>}</li>
</ol>
<a href="http://cssing.iatp.org.ua/examples/min-width/min1.html">смотреть пример</a>
Одна из проблем с этим методом описана ниже - заголок ВАЖНО!
<ul>
<li><a href="http://www.svendtofte.com/code/max_width_in_ie/">max-width in Internet Explorer (min-width)</a></li>
</ul>
<h3>ВАЖНО</h3>
Однако помните, что первый метод при некоторых Доктайпах вызывает подвисание IE WinXP SP1 при ресайзах окон. Смена доктайпа и еще пару примочек помогает. Например переход XHTML на HTML спасает.
Вот тут читайте подробнее - <a href="http://blog.unmatchedstyle.com/hacks/min-width-max-width-re-hacked">min-width, max-width re-hacked</a>.
<h3>Метод второй: два обертывающих DIV</h3>
Этот метод потребует добавления в код двух дополнительных DIV. Примерно так:
<ol class="code">
<li>&lt;div id="min-width"&gt;</li>
<li class="tab">&lt;div class="minwidth"&gt;</li>
<li class="tabtab">&lt;div class="container"&gt;</li>
<li class="tabtab">tut ku4a texta</li>
<li class="tabtab">&lt;/div&gt;</li>
<li class="tab">&lt;/div&gt;</li>
<li>&lt;/div&gt;</li>
</ol>
Тогда вот такой CSS нам сымитирует min-width для IE:
<ol class="code">
<li>/*для всех броузеров что понимают min-width */</li>
<li>#min-width {</li>
<li class="tab">width:50%; </li>
<li class="tab">min-width:400px; </li>
<li>}</li>
<li>/* для IE */</li>
<li>* html .minwidth {</li>
<li class="tab">border-left:400px solid #fff;/*min-width*/</li>
<li class="tab">position:relative; </li>
<li class="tab">float:left; </li>
<li class="tab">z-index:1;</li>
<li>}</li>
<li>* html .container {</li>
<li class="tab">margin-left:-400px; /*-min-width*/</li> 
<li class="tab">position:relative; </li>
<li class="tab">float:left; </li>
<li class="tab">z-index:2; </li>
<li>}</li>
</ol>
<a href="http://cssing.iatp.org.ua/examples/min-width/min.html">смотреть пример</a>
Если вкратце: то внутрь блока помещают другой, с границей равной минимальной ширине. Который и не дает ИЕ сжимать этот блок. Более подробное описание:
<ul>
<li><a href="http://www.cssplay.co.uk/boxes/minwidth.html">min-width for IE</a></li>
<li><a href="http://www.webreference.com/programming/min-width/">How to Use CSS to Solve min-width Problems in Internet Explorer</a></li>
</ul>
<h3><strong>Update:</strong> Метод 3: JavaScript</h3>
Для простоты приводимого кода я сделаю min-width для тэга body. Если необходимо реализовать для какого то блока - достаточно задать ID и использвать getElemetById.

Вобщем достаточно проинклюдить в страницу вот такой скрипт:
<ol class="code">
<li>var d = document;</li>
<li>var winIE = (navigator.userAgent.indexOf("Opera")==-1 && (d.getElementById &&  d.documentElement.behaviorUrns))  ? true : false;</li>
<li></li>
<li>function bodySize(){</li>
<li class="tab">if(winIE && d.documentElement.clientWidth) {</li>
<li class="tabtab">sObj = d.getElementsByTagName("body")[0].style;</li>
<li class="tabtab">sObj.width = (d.documentElement.clientWidth<<strong>760</strong>) ? "<strong>760px</strong>" : "<strong>100%</strong>";</li>
<li class="tab">}</li>
<li>}</li>
<li></li>
<li>function init(){</li>
<li class="tab">if(winIE) { bodySize(); }</li>
<li>}</li>
<li>onload = init;</li>
<li>if(winIE) { onresize = bodySize; }</li>
</ol>
В принципе аналогично первому методу с ескпрешонами - но этот вариант исключает подвисание броузера при ресайзе - поэтому если уж бить джаваскриптом, то лучше этим - хотя за определение броузера стыдно - но такова селяви... (подсмотрено живьем <a href="http://digital-web.com/">тут</a>)
</ol>
<h3>Заключение</h3>
В очередной раз убеждаемся что заставить ИЕ понимать можно все. Но не всегда это очевидно и стоит того.
<h3>Все ссылки</h3>
<ul>
<li><a href="http://blog.unmatchedstyle.com/hacks/min-width-max-width-re-hacked">min-width, max-width re-hacked</a></li>
<li><a href="http://www.svendtofte.com/code/max_width_in_ie/">max-width in Internet Explorer (min-width)</a></li>
<li><a href="http://www.cssplay.co.uk/boxes/minwidth.html">min-width for IE</a></li>
<li><a href="http://www.webreference.com/programming/min-width/">How to Use CSS to Solve min-width Problems in Internet Explorer</a></li>
</ul>
