---
title: "Аякс за 30 секунд"
date: "2005-11-28"
humanDate: "28 Nov, 2005"
permalink: "2005/11/28/rasmus-30-second-ajax-tutorial-on-russian/"
tags: 
  - "perevod"
comments: 
  -  author: "ganges"
     id: "2613"
     url: ""
     date: "2005-11-28 22:02:39"
     humandate: "28 Nov, 2005"
     content: | 
       "Тьюториал" - класс, АктивХ -ффу
       Сорри за ОТ

     email: "andrey.stefanenko@it.net.ua"

  -  author: "A.I."
     id: "2614"
     url: "http://www.sitnik.ru"
     date: "2005-11-29 08:25:33"
     humandate: "29 Nov, 2005"
     content: | 
       Кстати, есть и более простой способ AJAX'а:
       
       function sndReq(page) {
        document.write('');
       }
       
       Правда я не очень уверен, что он везде работает (в Mozilla и Opera 8 точно работает).

     email: "andsit@yandex.ru"

  -  author: "Rico+script.aculo.us at Staranger than Fiction"
     id: "2615"
     url: "http://shevtsov.fanstvo.com/2005/11/29/rico-scriptaculous/"
     date: "2005-11-29 09:29:09"
     humandate: "29 Nov, 2005"
     content: | 
       [...] Решил и я наконец познакомиться с Ajax’ом поближе… [...]

     email: ""

  -  author: "Attlant"
     id: "2622"
     url: "http://www.a3art.dp.ua/"
     date: "2005-11-29 15:03:28"
     humandate: "29 Nov, 2005"
     content: | 
       Можно исходнки в архиве?

     email: "design@a3art.dp.ua"

  -  author: "akella"
     id: "2623"
     url: "http://cssing.org.ua"
     date: "2005-11-29 15:15:03"
     humandate: "29 Nov, 2005"
     content: | 
       2AI:
       Ты наверно имел ввиду - <a href="http://dklab.ru/lib/Subsys_JsHttpRequest/" rel="nofollow">эту статью</a>?
       Мне, честно говоря, это не видится более простым способом. Кроме того в принципе корявоватым, хотя и более кроссбраузерным. Но это лишь ИМХО.
       2Attlant: я добавил линк

     email: "akella.a@gmail.com"

  -  author: "tobto_"
     id: "2624"
     url: "http://tobto.com.ua"
     date: "2005-11-29 17:28:18"
     humandate: "29 Nov, 2005"
     content: | 
       &gt;&gt; Это как использовать сложную ЦМС для сайта с 3 статическими страницами
       
       Это точно, относительно моего опыта с <a href="http://drupal.org" rel="nofollow">друпалом</a>. Вещь титаническая, но на локале 1.5 s перезагрузки на одну страницу. Странная вещь - я видел сайты серъезных людей, там где действительно было сделано 3 стр. на друпале. Вот это круто. Главное, - монументально.
       
       Относительно ajax: я пользуюсь постоянно IE5.5, Op9, FF0.9.3 и сравниваю результаты. Заметил, что ресурсы сделанные на AJAX обламываются скорее, чем обычные. Типично, выскакивает алерт: "Не могу послать HttpRequest". Возникает впечатление, что ajax хочет стабильной связи - иначе посыл броузера зависает. И это при выделенке.

     email: "info@eurosong2006.net"

  -  author: "mcbn"
     id: "2625"
     url: ""
     date: "2005-11-30 00:31:15"
     humandate: "30 Nov, 2005"
     content: | 
       occide se de parietam.. XML sockets выброси на помойку. А вот куда идти читать: http://dklab.ru/lib/Subsys_JsHttpRequest

     email: "nosp@m.lol"

  -  author: "Антон Бо"
     id: "2626"
     url: "http://aj.active.by"
     date: "2005-11-30 09:28:22"
     humandate: "30 Nov, 2005"
     content: | 
       Шустренький, маленький (JS меньше килобайта), до тупого простой, сменщик innerHTML — AHAH: http://microformats.org/wiki/rest/ahah :)
       
       Хоть я и далёк от JS, но не вижу причин не пихать в запрос параметры, а с той стороны иметь, например, php. Поправьте, если чего.

     email: "aj@tut.by"

  -  author: "mcbn"
     id: "2627"
     url: ""
     date: "2005-11-30 10:55:41"
     humandate: "30 Nov, 2005"
     content: | 
       Антон - в дестку(е) !

     email: "nosp@m.lol"

  -  author: "mcbn"
     id: "2628"
     url: ""
     date: "2005-11-30 10:57:19"
     humandate: "30 Nov, 2005"
     content: | 
       сказано же, что XMLHttpRequest менее практичен. ActiveX как никак. А на dklab.ru сделано 2 варианта в одном флаконе.

     email: "nosp@m.lol"

  -  author: "akella"
     id: "2629"
     url: "http://cssing.org.ua"
     date: "2005-11-30 11:32:58"
     humandate: "30 Nov, 2005"
     content: | 
       <blockquote>сказано же, что XMLHttpRequest менее практичен</blockquote>
       Мне это видится воркараундом - а не бест практис.. Что значит менее практичен? Видимо этот вопрос исчерпывается Оперой и отключенным ActiveX.
       К тому же та библиотека <strong>использует</strong> XMLHttpRequest если он доступен. А поддерживать совсем старые броузеры невыгодно из-за других расхождений в понимании ДЖС.
       Это все равно что юзать всякие HTML атрибуты вместо CSS. XMLHttpRequest для того только и был придуман. А писать &lt;script&gt; временное решение для некоторых броузеров.
       
       К тому же мне совершенно неинтересно было предлагать какую то супер библиотеку-скрипт которая решит все ваши проблемы.
       Такие решения по умолчанию неоптимальны. К чему вам библиотека если можно обойтись половиной ее функций? Зачем вам ЦМС если можно создать три статических страницы?
       
       Как раз наоборот, я хотел показать то, с чего можно начать знакомиться с аяксом - я больше чем уверен что любое приложение на базе библиотеки займет куда больше байт чем мое заточеное под задачу - без ничего лишнего. К тому же будет труднее для понимания.
       
       2 Антон Бо: спасибо за линк - в принцпе это одно и тоже с тем что описано в статье - просто развитая мысль - и по другому скомпонованы функции. Кому как удобнее..
       <blockquote>Хоть я и далёк от JS, но не вижу причин не пихать в запрос параметры, а с той стороны иметь, например, php. Поправьте, если чего.</blockquote>
       Видимо ты не до конца понял что и там и у меня они пихаются абсолютно одинаково...
       
       Еще раз скажу: Это не очередная библиотека - это тьюториал для начинающих. Если вам легче брать библиотеку(UltraUniversalAJAX) и разбираться в ней - пожалуйста - некоторым(мне :)) проще разобраться от самого начала и писать свои решения и не использовать библиотеки...

     email: "akella.a@gmail.com"

  -  author: "mcbn"
     id: "2633"
     url: ""
     date: "2005-12-01 13:16:30"
     humandate: "01 Dec, 2005"
     content: | 
       Дело в том, что ActiveX блокируют много пользователей собственноручно. Разговор уже не о том, что Опера такая-секая. Во-вторых, ActiveX блокируется по умолчанию множеством МСЭ ( персональных, конечно ). Да и IE последних версий ругается. 
       
       Нет, на самом деле, детский сад обсуждать ActiveX компноненты. Всё уже пережёвано до неузнаваемости. Тот вариант, который я предложил, хорош тем, что в обсуждаемом классе реализуется, и ActiveX-управление, и, пардон, не-ActiveX.
       
       Да и "разбираться" в них никто не заставляет. Не хотите - сами напишите.

     email: "nosp@m.lol"

  -  author: "akella"
     id: "2634"
     url: "http://cssing.org.ua"
     date: "2005-12-01 14:23:43"
     humandate: "01 Dec, 2005"
     content: | 
       Понятно что тот универсальнее - но далеко не такой легкий для понимания сразу. И все же - ну некрасивый он. А это собссно перевод очень хорошего как по мне тьюториала для начала работы. Когда уж заморочимся на поддерживаемости - можно и тот использовать.
       
       Кстати 
       <blockquote>Дело в том, что ActiveX блокируют много пользователей собственноручно.</blockquote>
       Есть ли статистика? Мне почему-то кажется что проблема отключенного джаваскрипта родственна в статистическом смысле этой.
       То есть очень сильно меньше 1%. Лишь кажется - если бы статистику...

     email: "akella.a@gmail.com"

  -  author: "mcbn"
     id: "2635"
     url: ""
     date: "2005-12-01 14:56:30"
     humandate: "01 Dec, 2005"
     content: | 
       1. Ну, уж если сложно...
       2. Конечно, статистика! Не от былды же говорю.

     email: "nosp@m.lol"

  -  author: "akella"
     id: "2636"
     url: "http://cssing.org.ua"
     date: "2005-12-01 15:16:49"
     humandate: "01 Dec, 2005"
     content: | 
       ну... ссылка на статистику?
       
       Я и так понял что ты убежден что их много с отключенным ActiveX.
       Мне интересна статистика откуда ты почерпнул такую информацию. Я к сожалению не смог найти...
       Я не отрицаю - но мне интересно сколько и по чьим данным?

     email: "akella.a@gmail.com"

  -  author: "mcbn"
     id: "2637"
     url: ""
     date: "2005-12-01 16:47:50"
     humandate: "01 Dec, 2005"
     content: | 
       Вот ещё.. ссылки искать буду. Прийду домой, гляну в хистори, если успею %)

     email: "nosp@m.lol"

  -  author: "akella"
     id: "2638"
     url: "http://cssing.org.ua"
     date: "2005-12-05 10:58:38"
     humandate: "05 Dec, 2005"
     content: | 
       Без статистики - все пустые слова...

     email: "akella.a@gmail.com"

  -  author: "mcmx"
     id: "2655"
     url: ""
     date: "2005-12-11 22:34:00"
     humandate: "11 Dec, 2005"
     content: | 
       Поправте мня, если я не прав:
       В статье показан скорее _ПОДХОД_ чем _КОНКРЕТНАЯ РЕАЛИЗАЦИЯ_ , а DK либа - это уже некое решение, предусматривающее реальную ситуацию.
       2akella - Статья понравилась, и оч много идей подкинула по моему сайту. 
       однако в опере на ukrnet не работает однако совершенно.... :)

     email: "mcmx@myphoto.com.ua"

  -  author: "akella"
     id: "2656"
     url: "http://cssing.org.ua"
     date: "2005-12-12 01:28:41"
     humandate: "12 Dec, 2005"
     content: | 
       Конечно подход. Или скорее путь по построению библиотеки под конкретные нужды. или даже просто начало знакомства с технологией с самого начала а не с библиотек.
       
       А для оперы надо добавить создание еще одного обьекта в функцию createRequestObject - msxml2 или типа того. Потому и не работает - старался сделать максимально приближенным к статье...

     email: "akella.a@gmail.com"

  -  author: "mcmx"
     id: "2657"
     url: ""
     date: "2005-12-12 21:10:24"
     humandate: "12 Dec, 2005"
     content: | 
       У меня опера 8.5 стоит, в ней XMLHttpRequest работает. Но одна деталь, которая меня бесит...
       В ответ на navigator.appName она нагло заявляет, что она 'Microsoft Internet Explorer'(!!!) 
       
       поэтому немного поправленый кусок кода вполне работает (по крайней мере в 8.5)
       
       function createRequestObject() {
        var ro;
        var userAgent=navigator.userAgent;
        if (userAgent.indexOf('MSIE') != -1)
        {
        if (userAgent.indexOf('Opera') != -1) // Собственно интересуемся "А не опера ли ты часом?"
        {
        ro = new XMLHttpRequest();
        }
        else
        {
        ro = new ActiveXObject('Microsoft.XMLHTTP');
        }
        }
        else
        {
        ro = new XMLHttpRequest();
        }
        return ro;
       }
       
       Все остальное - как у тебя.

     email: "mcmx@myphoto.com.ua"

  -  author: "akella"
     id: "2658"
     url: "http://cssing.org.ua"
     date: "2005-12-13 12:36:29"
     humandate: "13 Dec, 2005"
     content: | 
       Если уж говорить о кроссбразуерных- то вот такой код "общепринят":
       <pre>var xmlHttp = false;
       /*@cc_on @*/
       /*@if (@_jscript_version &gt;= 5)
       try {
        xmlHttp = new ActiveXObject('Msxml2.XMLHTTP');
       } catch (e) {
        try {
        xmlHttp = new ActiveXObject('Microsoft.XMLHTTP');
        } catch (e2) {
        xmlHttp = false;
        }
       }
       @end @*/
       
       if (!xmlHttp &amp;&amp; typeof XMLHttpRequest != 'undefined') {
        xmlHttp = new XMLHttpRequest();
       }</pre>
       взято с <a href="http://www-128.ibm.com/developerworks/web/library/wa-ajaxintro1.html?ca=dgr-lnxw01MasterAJAX" rel="nofollow">отсюда</a>

     email: "akella.a@gmail.com"

  -  author: "mcmx"
     id: "2660"
     url: ""
     date: "2005-12-13 14:01:28"
     humandate: "13 Dec, 2005"
     content: | 
       Небуду стучать пальцами об двери, я не слишком силен в JS :)
       Я вообще дизайнер и старый сионист, PHP-шник по надобности. :)
       А за инфу спаибо, буду пробовать.

     email: "mcmx@myphoto.com.ua"

  -  author: "CB"
     id: "2661"
     url: "http://sudoku.org.ua"
     date: "2005-12-13 14:15:59"
     humandate: "13 Dec, 2005"
     content: | 
       Мой последний вариант
       <pre>function createRequestObject()
       {
        var ro;
       
        if (window.XMLHttpRequest) { ro = new XMLHttpRequest(); }
        else {
        ro = new ActiveXObject('Msxml2.XMLHTTP');
        if(!ro) { ro = new ActiveXObject('Microsoft.XMLHTTP'); }
        }
       
        return ro;
       }</pre>

     email: "serhiy_voloshyn@gmail.com"

  -  author: "mcmx"
     id: "2662"
     url: ""
     date: "2005-12-13 14:56:02"
     humandate: "13 Dec, 2005"
     content: | 
       И всетаки интересно, какой модели придерживается опера.

     email: "mcmx@myphoto.com.ua"

  -  author: "CB"
     id: "2664"
     url: "http://sudoku.org.ua"
     date: "2005-12-13 16:02:03"
     humandate: "13 Dec, 2005"
     content: | 
       ro = new ActiveXObject('Msxml2.XMLHTTP');
       Эта строка для Опер (в моем варианте) Имхо по имени браузер определят не очень надежно

     email: "serhiy_voloshyn@gmail.com"

  -  author: "mcmx"
     id: "2667"
     url: ""
     date: "2005-12-14 14:14:19"
     humandate: "14 Dec, 2005"
     content: | 
       по appName - ненадежно. по userAgent - вполне :)
       В моем примере какраз по имени отсекает достаточно точно.
       просто в последних операх какого то ляда они стали притворятся IE .
       
       Твой вариант компактнее - спору нет :)
       но он плодит сообщения об ошибках у фокса :(

     email: "mcmx@myphoto.com.ua"

  -  author: "CB"
     id: "2668"
     url: "http://sudoku.org.ua"
     date: "2005-12-14 16:40:35"
     humandate: "14 Dec, 2005"
     content: | 
       2 mcmx: А можно поподробнее об ошибках у фокса. У меня все вроде гладко работает (код выдран с рабочего скрипта на судоку.орг.уа), ЖС-консоль девственно чиста :)

     email: "serhiy_voloshyn@gmail.com"

  -  author: "mcmx"
     id: "2669"
     url: ""
     date: "2005-12-14 18:08:29"
     humandate: "14 Dec, 2005"
     content: | 
       Ой... сори, я бок запорол... поправил - все ок...

     email: "mcmx@myphoto.com.ua"

  -  author: "CB"
     id: "2672"
     url: "http://sudoku.org.ua"
     date: "2005-12-23 17:42:43"
     humandate: "23 Dec, 2005"
     content: | 
       http.readyState:
       0 = uninitialized
       1 = loading
       2 = loaded
       3 = interactive
       4 = complete
       
       tnx to DiGiTAL

     email: "serhiy_voloshyn@gmail.com"

  -  author: "Илья Барков"
     id: "2699"
     url: "http://www.barkov.net/"
     date: "2006-01-09 20:13:13"
     humandate: "09 Jan, 2006"
     content: | 
       Спасибо за перевод! То, что я искал!

     email: "ilyaabarkov.net"

  -  author: "Jeje"
     id: "2742"
     url: ""
     date: "2006-01-22 14:06:07"
     humandate: "22 Jan, 2006"
     content: | 
       Опера предваряется IE скорее всего из-за настроек в ней
       Зайдите в Tools-&gt;Preferences-&gt;Advanced-&gt;Network-&gt;Browser Identification

     email: "jeje@mail.ru"

  -  author: "intenter"
     id: "2905"
     url: ""
     date: "2006-03-23 19:11:44"
     humandate: "23 Mar, 2006"
     content: | 
       Если тема интересна, то вот еще пара очень простых примеров с описанием:
       
       <a href="http://intenter.ru/me/articles/aja.jsp" rel="nofollow">AJA - AJAX без XML</a>
       <a href="http://intenter.ru/me/articles/poll.jsp" rel="nofollow">Опрос с помощью AJAX</a>

     email: "intenter@list.ru"

  -  author: "CB's blog"
     id: "2918"
     url: "http://sudoku.org.ua/rus/blog/2006/03/30/deltablerows2/"
     date: "2006-03-30 15:21:58"
     humandate: "30 Mar, 2006"
     content: | 
       [...]перевод можно найти тут. Уверен, что уже после того как вы их прочитаете, сразу возникнет желание чтото реализовать и самому [...]

     email: ""

  -  author: "SOb"
     id: "3268"
     url: "http://intranet"
     date: "2006-05-20 13:27:24"
     humandate: "20 May, 2006"
     content: | 
       Замечу, что на сайте http://cssing.org.ua/ajax/ блок с содержимым новости было бы здорово позиционировать относительно координат мыши (clientX, clientY). Ниже на 10px, например.

     email: "sob_s@mail.ru"

  -  author: "Gart"
     id: "4157"
     url: ""
     date: "2006-08-02 14:11:40"
     humandate: "02 Aug, 2006"
     content: | 
       А кто подскажет: при возврате ответа с сервера кирилица выводится кракозабрами? как это подлечить?

     email: "art_g@mail.ru"

  -  author: "akella"
     id: "5369"
     url: "http://cssing.org.ua"
     date: "2006-10-01 14:34:45"
     humandate: "01 Oct, 2006"
     content: | 
       Проставь в php скрипте который отправляет ответ - кодировку.
       функцией <code>header</code>, например:
       
       header("Content-type: text/html; charset=UTF-8");

     email: "akella.a@gmail.com"

  -  author: "Vladson"
     id: "5379"
     url: "http://vladson.com/"
     date: "2006-10-02 04:03:25"
     humandate: "02 Oct, 2006"
     content: | 
       akella почини RSS у каментов, у тебя там ампрессанды не фильтруются... (в "title")

     email: "dkflbk@nm.ru"

  -  author: "KeTal"
     id: "6831"
     url: "http://home.ketal.ru"
     date: "2006-12-24 00:20:00"
     humandate: "24 Dec, 2006"
     content: | 
       Респект! То что надо!

     email: "noreply@ketal.ru"

  -  author: "Костя"
     id: "8145"
     url: "http://site3k.net/"
     date: "2007-02-10 16:02:58"
     humandate: "10 Feb, 2007"
     content: | 
       mcbn сказал(а) 
       "XMLHttpRequest менее практичен. ActiveX как никак"
       
       А вот Аякс без ActiveX и XMLHttpRequest. (http://webdesign.site3k.net/consulting/ajax.html)
       
       mcmx сказал(а) 
       "опера... она нагло заявляет, что она ‘Microsoft Internet Explorer’"
       
       Это зависит от того, как ты ее настроиш. Но вот точное определение браузера. Однако в случае Аякса, лучше ориентироваться не на имя браузера, а на то, работает модуль, или нет. То есть:
       
        if(window.XMLHttpRequest){тут код}

     email: "discoveri@narod.ru"

  -  author: "Powermic"
     id: "8855"
     url: ""
     date: "2007-02-26 17:56:54"
     humandate: "26 Feb, 2007"
     content: | 
       Очень полезная статья, автору, переводчику и постерам мега респект.

     email: "powermic@rambler.ru"

  -  author: "Vladson"
     id: "8882"
     url: "http://vladson.com/"
     date: "2007-02-27 09:06:25"
     humandate: "27 Feb, 2007"
     content: | 
       Мне на эту тему больше нравится http://developer.mozilla.org/en/docs/AJAX:Getting_Started и просто и информативно...

     email: "dkflbk@nm.ru"

  -  author: "Sliper"
     id: "15358"
     url: "http://wm-ads.ru"
     date: "2010-02-05 14:31:51"
     humandate: "05 Feb, 2010"
     content: | 
       Мне помогло следующее (кодировка всего сайта windows-1251): в корневом .htaccess нужно добавить следующую стоку 
       
       AddDefaultCharset windows-1251
       
       После этого вопросительные знаки пропали...

     email: "sliper@mail.ru"

  -  author: "dark-demon"
     id: "10963"
     url: "http://dark-demon.nm.ru/web/samples/xhtml/index.xml#jframes"
     date: "2007-05-24 22:50:56"
     humandate: "24 May, 2007"
     content: | 
       ещё один ультракомпактнокроссбраузерный аякс ^_^
       http://darkodemon.blogspot.com/2007/05/blog-post_5931.html

     email: "dark-demon@mail.ru"

  -  author: "Max"
     id: "10986"
     url: "http://-"
     date: "2007-06-20 08:32:03"
     humandate: "20 Jun, 2007"
     content: | 
       Здравствуйте.
       Проблема ...
       
       function handleResponse() {
        if(http.readyState == 4){
        var response = http.responseText;
        document.getElementById('foo').innerHTML = response;
        }
       }
       
       ... после выполнения замес-то слов вопросительные знаки присылает, почему?

     email: "chuvak47@yandex.ru"

  -  author: "akella"
     id: "10988"
     url: "http://cssing.org.ua"
     date: "2007-06-20 16:05:47"
     humandate: "20 Jun, 2007"
     content: | 
       почитайте комментарий #36

     email: "akella.a@gmail.com"

layout: "layouts/post.njk"
excerpt: "Перевожу заметку с которой я начал свое знакомство с аяксом.
Находится на <a href=\"http://rajshekhar.net/blog\">сайте Rasmus'a</a> -  <a href=\"http://rajshekhar.net/blog/archives/85-Rasmus-30-second-AJAX-Tutorial.html\">Rasmus' 30 second AJAX Tutorial</a>.
Мой вольный перевод."
---

Перевожу заметку с которой я начал свое знакомство с аяксом.
Находится на <a href="http://rajshekhar.net/blog">сайте Rasmus'a</a> -  <a href="http://rajshekhar.net/blog/archives/85-Rasmus-30-second-AJAX-Tutorial.html">Rasmus' 30 second AJAX Tutorial</a>.
Мой вольный перевод.<!--more-->
Вообще сам Аякс я считаю немного обманом. Многие использовали те же самые приемы задолго до того как они вдруг стали "Аяксом". И эти вещи совсем не такие сложные как многие считают. Вот простой пример из одного из моих приложений.
Сначала Javascript:
<pre>
function createRequestObject() {
    var ro;
    var browser = navigator.appName;
    if(browser == 'Microsoft Internet Explorer'){
        ro = new ActiveXObject('Microsoft.XMLHTTP');
    }else{
        ro = new XMLHttpRequest();
    }
    return ro;
}

var http = createRequestObject();

function sndReq(action) {
    http.open('get', 'rpc.php?action='+action);
    http.onreadystatechange = handleResponse;
    http.send(null);
}

function handleResponse() {
    if(http.readyState == 4){
        var response = http.responseText;
        var update = new Array();

        if(response.indexOf('|' != -1)) {
            update = response.split('|');
            document.getElementById(update[0]).innerHTML = update[1];
        }
    }
}
</pre>
Этот код создает обьект запроса, сам запрос  и функцию для его принятия и распарсивания(по названиям, собственно, нетрудно догадаться). Для использования вам нужно  включить этот скрипт в вашу страницу. (<code>&lt;script type="text/javascript" src="js.js"&gt;&lt;/script&gt;</code>)
Теперь для того чтобы послать запрос нужно его прицепить к какому-нибудь событию. Например onclick или поместив прямо в href вот так: 
<ol class="code">
<li> &lt;a href="javascript:sndReq('foo')"&gt;[foo]&lt;/a&gt;</li>
</ol>
Это означает что при клике на эту ссылку будет отослан вот такой запрос <strong>rpc.php?action=foo</strong>.

В rpc.php у вас может быть примерно такой код:
<ol class="code">
<li>switch($_REQUEST['action']) {</li>
<li class="tab">case 'foo': /*...action=foo...*/</li>
<li class="tabtab">/*<strong> тут например запрос к базе</strong>*/</li>
<li class="tabtab">echo "foo|foo done";</li>
<li class="tabtab"> break;</li>
<li class="tab">...</li>
<li>}</li>
</ol>
Теперь обратим внимание на handleResponse. Оно распарсивает строку "foo|foo done"  и разделяет ее по символу  '|'. Причем использует то что было до  '|' - как id блока в HTML, а то что после - как новый innerHTML для этого блока. В данном случае, если у вас на странице есть вот такой HTML:
<ol class="code">  
<li>&lt;div id="foo"&gt;</li>
<li>&lt;/div&gt;</li>
</ol>
То как только вы кликните на ссылку, он динамически изменится на:
<ol class="code">  
<li>&lt;div id="foo"&gt;</li>
<li>foo done</li>
<li>&lt;/div&gt;</li>
</ol>
Вот собственно и все. Остальное лишь надстройка над этим простым скриптом. Заменяйте мой простой ответ от сервера "id|text" на более богатый формат XML, и делайте запрос сложнее чем просто с одной переменной. Перед тем как вы слепо установите одну из тысяч "AJAX" библиотек попробуйте сами добавить в этот скрипт нужный вам функционал, чтобы понять как именно оно работает и усложнить его ровно настолько насколько это вам нужно. Очень часто нужно не намного больше этого моего примера.

Обобщить этот подход, например для отсылки нескольких переменных, было бы очень просто, примерно так:
<ol class="code">
<li>function sndReqArg(action,arg) {</li>
<li class="tab">http.open('get', 'rpc.php?action='+action+'&amp;arg='+arg);</li>
<li class="tab">http.onreadystatechange = handleResponse;</li>
<li class="tab">http.send(null);</li>
<li>}</li>
</ol>

А функцию handleResponse можно легко расширить для более интересных целей, чем просто замещение содержимого ДИВа.

Автор - <a href="http://rajshekhar.net/blog">Rasmus</a>
<h3>В конце</h3>
Вот такая вот статейка. На ее базе мне например хватило 2Кб  скрипта для создания вот <a href="http://cssing.org.ua/ajax/">такой вот фичи для укр.нета</a> (<a href="http://cssing.org.ua/examples/jx/u-jx.rar">исходники</a>). Не без помощи <a href="http://sudoku.org.ua/rus/">CB</a> правда. :) Джаваскриптер из меня все же слабенький.
Прошу прощения за местами косноязычный перевод - я старался :). Считаю это одним из лучших тюториалов для начала работы с аяксом. 

Хотя бы потому, что лично мне претит использовать все эти навороченные библиотеки. Это как использовать сложную ЦМС для сайта с 3 статическими страницами. Такие вот ассоциации. И это не говоря о пушках и воробьях. 

<strong>Ваше мнение по поводу тюториала приветствуется!</strong>
