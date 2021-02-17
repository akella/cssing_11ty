---
title: "Простой тултип или всплывающая подсказка"
date: "2006-02-15"
humanDate: "15 Feb, 2006"
permalink: "2006/02/15/css-tooltips/"
tags: 
  - "xhtmlcss"
comments: 
  -  author: "alex-and-r"
     id: "2766"
     url: "http://www.intruder.ru/"
     date: "2006-02-15 16:11:40"
     humandate: "15 Feb, 2006"
     content: | 
       Хм...
       
       Вопрос первый: семантическая корректность. Как с ней быть? Вы не брали это в расчет?
       Вопрос второй: seo. Там же четко про бан в комментах говорится по ссылке на пример поисковой оптимизации, нет?
       Вопрос третий (собственно больше всего интересующий, а остальные так, риторические): значение "23" для св-ва "z-index" выбрано просто наобум или с каким-то умыслом?

     email: "alexandr@gmail.com"

  -  author: "akella"
     id: "2767"
     url: "http://cssing.org.ua"
     date: "2006-02-15 17:10:36"
     humandate: "15 Feb, 2006"
     content: | 
       Собсно <strong>ответ номер 1</strong>:Семантическая корректность в смысле чтения читателями экранов? Если вспомнить о ней, можно использовать псевдоселекторы :after :before и раставить скобки около текста внутри спана, примерно так:
       
       a.tt span:before { content: "(" }
       a.tt span:after{ content: ")" }
       
       Для уменьшения интонации можно вместо span использовать small например. Какой именно недостаток в семантике пояснения к тексту ссылки здесь, может я неправильно понял?
       
       <strong>Ответ 2</strong>: ну в том посте на который я сослался безусловно метод мог быть совсем корректен и семантичен - там юзера вообще не видели того текста и соответственно туда могли писать что угодно. А в данном случае нужно писать осмысленную информацию и я не вижу причин банить пояснение к ссылке. Наверно потому что их нет. Это обычный контент. Все в рамках, имхо. Банят если туда вписать 10 кейвордов и так раз 20 на странице. Здесь же все по смыслу должно быть - иначе, что за прикол юзеру читать ваше семантическое ядро.
       
       <strong>Ответ 3</strong>: в данном случае важно лишь что 22 меньше чем 23. Оба они больше 0 и меньше 256. Значение з-индекс указывает какой блок должен быть отображен поверх какого. У кого меньше тот и главный. :)
       
       Конкретные значения выбраны исходя из возраста автора поста.

     email: "akella.a@gmail.com"

  -  author: "Vladson"
     id: "2768"
     url: "http://dkflbk.nm.ru/"
     date: "2006-02-15 17:47:00"
     humandate: "15 Feb, 2006"
     content: | 
       По поводу №2 (ИМХО):
       
       В первую очередь это такой-же контент как и любой другой, то что он скрыт до наведения на него мышью не значит что он скрыт совсем а стало быть никаких причин для бана нету.
       
       Если какой-то поисковик будет банить за такое то это его проблемы а не мои, я как чесный дизайнюк делаю дизайн для людей а не для поисковых машин, так что если им что-то не нравится пускай идут "наффик".

     email: "dkflbk@nm.ru"

  -  author: "ganges"
     id: "2769"
     url: "http://idcontent.com/"
     date: "2006-02-15 18:21:08"
     humandate: "15 Feb, 2006"
     content: | 
       Насчет семантики, с моей точки зрения там вообще нет проблем - span семантики не несет. стало быть объяснение это просто продолжение ссылки, чем оно и есть. Для скринридеров, опятьже имхо, это только хорошо. - лучше чем без объяснения - оно прочитает LINK - и дальше раскажет о чем этот линк.
       
       По поводу бана - если за такие вещи Гугл и будет банить, то только если туда спам вписывать повторяющийся. Это просто ссылка.
       
       По поводу usability
       В твоем примере тултип перекрывает две нижеследующие ссылки и надо делать дополнительное движение. чтобы от него избавиться (Linux FF) ИМХО, в тексте это ОК, (как насчет onfocus :) а в меню - либо отказаться, либо позиционировать тултип в строке со ссылкой, предварительно развинув с помощью line-height строку

     email: "andrey.stefanenko@gmail.com"

  -  author: "akella"
     id: "2770"
     url: "http://cssing.org.ua"
     date: "2006-02-15 19:12:04"
     humandate: "15 Feb, 2006"
     content: | 
       2Ganges: Пожалуй ты прав, можно к :hover добавить еще и :focus или как там оно.. :) Но это уже мелочи.
       
       А с координатами нужно играться конечно у меня там неидеально вышло. Вот с календарем гораздо приятнее получилось, и без лишних движений. Наверно нужно больше в сторону сдвигать - в этом секрет успеха.

     email: "akella.a@gmail.com"

  -  author: "Tomaz"
     id: "2771"
     url: ""
     date: "2006-02-15 19:49:26"
     humandate: "15 Feb, 2006"
     content: | 
       В Опере 8.5 тултип ведет себя как-то странно: он не исчезает полностью, часть его остается видимой.

     email: "igor.baluev@gmail.com"

  -  author: "akella"
     id: "2772"
     url: "http://cssing.org.ua"
     date: "2006-02-15 20:28:23"
     humandate: "15 Feb, 2006"
     content: | 
       Нда, какой то странный глюк оперы :(.
       Он проявляется при одновременном использовании z-index и position:absolute;
       
       При убирании з-индекс глюк исчезает, но опять же приходится задавать position:relative для a.tt а не для a.tt:hover. И тут всплывают проблемы с ИЕ... Приходится хакать. Короче говоря надо выпустить ДВА варианта тултипов для разных ситуаций на странице. Странно что опера так странно себя ведет :(.
       
       Завтра сделаю апдейт.

     email: "akella.a@gmail.com"

  -  author: "Владимир Яшников"
     id: "2773"
     url: "http://www.yashnikov.ru"
     date: "2006-02-15 23:43:24"
     humandate: "15 Feb, 2006"
     content: | 
       <a href="http://www.phoenity.com/newtedge/element_hover/">Здесь</a> можно найти ещё несколько интересных примеров.

     email: "yashnikov@gmail.com"

  -  author: "uggallery"
     id: "2778"
     url: "http://uggallery.audiopeace.ru"
     date: "2006-02-17 17:31:08"
     humandate: "17 Feb, 2006"
     content: | 
       Еще неприятный момент: <a href="http://uggallery.narod.ru/1/ccsingtooltip.png" rel="nofollow">на скриншоте</a>. Курсор с левого края, тултип -- с правого, и не умещается на экране. Но простота -- это действительно, сила. Если правильно учесть ограниченность метода. Или сделать вариант с "немножко JavaScript".
       
       С точки зрения юзабилити, у меня один общий вопрос к любым нестандартным тултипам: насколько их использование вообще оправдано? Но это нужно решать в каждом конкретном случае, отдельно.

     email: "uggallery@yandex.ru"

  -  author: "akella"
     id: "2780"
     url: "http://cssing.org.ua"
     date: "2006-02-17 19:49:27"
     humandate: "17 Feb, 2006"
     content: | 
       Да, спасибо, я и не ожидал.
       Пожалуй стоит обезопасивать большими отступами такие "обьекты" :). Спасибо еще раз.

     email: "akella.a@gmail.com"

  -  author: "доброход"
     id: "2781"
     url: ""
     date: "2006-02-18 12:45:44"
     humandate: "18 Feb, 2006"
     content: | 
       а не могли бы кинуть ссылку на "непростой" тултип? с кучей JS? Спасибо!

     email: "dobrohod@neo-lit.ru"

  -  author: "Dmitry"
     id: "2782"
     url: "http://borr.wordpress.com"
     date: "2006-02-18 16:30:06"
     humandate: "18 Feb, 2006"
     content: | 
       Я тоже как-то занимался аналогичными подсказками http://borr.nm.ru/pub/xml/tocmenu.xml - здесь основной пример. А вообще весь сайт был сделан с упором на подобные подсказки. И еще - есть подозрение, что мой пример не работает в Ие и других сотоварищах, так как кроме mozilla я в глаза вообще никого не видел, зато у меня полупрозрачный фон и скругленные углы :) . Ваш пример должен быть более кросплатформенным.

     email: "qborrd@gmail.com"

  -  author: "akella"
     id: "2784"
     url: "http://cssing.org.ua"
     date: "2006-02-19 15:40:59"
     humandate: "19 Feb, 2006"
     content: | 
       <strong>2 доброход:</strong> Вот здесь - <a href="http://htmlcoder.visions.ru/JavaScript/?11" rel="nofollow">Всплывающая подсказка (tooltip) с использованием DOM</a> - более сложный вариант.
       
       А так же не следует забывать о <a href="http://kryogenix.org/code/browser/nicetitle/" rel="nofollow">nicetitles</a> (<a href="http://cssing.org.ua/2004/09/22/nice-titles/" rel="nofollow">и на русском</a>)
       
       <strong>2 Dmitry:</strong> спасибо за интересный пример - это наверно наше кодерское будущее... :)

     email: "akella.a@gmail.com"

  -  author: "Double"
     id: "2786"
     url: ""
     date: "2006-02-19 20:01:10"
     humandate: "19 Feb, 2006"
     content: | 
       В Opera 8.5.1 глючит пример. Поэтому ниасилил (т.е. дальше читать не стал :)

     email: "doppeltes@gmail.com"

  -  author: "CB"
     id: "2789"
     url: "http://sudoku.org.ua/rus/blog"
     date: "2006-02-20 12:21:45"
     humandate: "20 Feb, 2006"
     content: | 
       Мой вариант:
       
       http://sudoku.org.ua/rus/blog/examples/tt/

     email: "serhiy_voloshyn@gmail.com"

  -  author: "akella"
     id: "2788"
     url: "http://cssing.org.ua"
     date: "2006-02-20 11:32:20"
     humandate: "20 Feb, 2006"
     content: | 
       Я собственно так и написал - что для оперы 8.51 нужен отдельный пример в силу корявости данного броузера в области position:absolute, он никак не может асилить данную простую технику. Как я и написал достаточно убрать z-index и все работает.
       
       Вобщем то Вам проще было написать ниасилил видимо ) чем все-таки асилить сей огромный пост. :)
       В любом случае - отличный коммент :))
       
       Ну а во вторых глючит не везде... Потому я и написал что для разных случаев разную технику нужно использовать.
       
       Единственное решение которое я пока вижу - отдавать отдельный ЦСС для ВСЕХ бразуеров кроме Оперы - имхо <strong>слишком</strong> много чести - все же это не жизненно важный функционал, а прикольная фича - которую пускай видят только обладатели доработанных броузеров :P

     email: "akella.a@gmail.com"

  -  author: "akella"
     id: "2790"
     url: "http://cssing.org.ua"
     date: "2006-02-20 12:30:51"
     humandate: "20 Feb, 2006"
     content: | 
       По адресу http://cssing.org.ua/examples/csstooltip/index1.html - находится пример для оперы - пришлось пожертвовать отображением тултипов поверх других (тултипистых)ссылок на странице.
       
       Однако если важна поддержка и никак не уйти от оперы...

     email: "akella.a@gmail.com"

  -  author: "UGgallery   &raquo; Tooltips"
     id: "2791"
     url: "http://uggallery.audiopeace.ru/?p=125"
     date: "2006-02-20 14:06:33"
     humandate: "20 Feb, 2006"
     content: | 
       [...] Tooltips
       20 Фев. 2006
       
       Простой тултип или всплывающая подсказка (от cssing)
       
       Без Javascript. Только HTML и CSS.[...]

     email: ""

  -  author: "(v)"
     id: "2843"
     url: "http://www.vady.kiev.ua/"
     date: "2006-03-02 05:10:58"
     humandate: "02 Mar, 2006"
     content: | 
       Жаваскрипт?! Да почему бы и нет, хватит жить в архаичном мире!
       
       http://www.dustindiaz.com/sweet-titles

     email: "vady@vady.kiev.ua"

  -  author: "akella"
     id: "2844"
     url: "http://cssing.org.ua"
     date: "2006-03-02 13:59:20"
     humandate: "02 Mar, 2006"
     content: | 
       Как по мне то каждый выбирает сам :) Не вижу ничего архаичного в неупотреблении джаваскрипта для таких простецких эффектов.

     email: "akella.a@gmail.com"

  -  author: "rodem"
     id: "2881"
     url: ""
     date: "2006-03-10 11:50:51"
     humandate: "10 Mar, 2006"
     content: | 
       http://www.bosrup.com/web/overlib/
       Собственно использую аж с 2000-го года. 36 кб js - работает везде.

     email: "roman.demenkov@gmail.com"

  -  author: "sazuke"
     id: "2920"
     url: "http://#"
     date: "2006-04-03 11:43:15"
     humandate: "03 Apr, 2006"
     content: | 
       все здорово!! только хотел я это применить к выпадающему списку типа 
       
       
       
        не проходит )) Разбираю css на примерах и спецификацию почитываю )
        Может поможет кто ?
       p.s. Как предполагаю, нужно искать в направлении прописывания классов для

     email: "xmoutionx@gmail.com"

  -  author: "gordi"
     id: "2938"
     url: ""
     date: "2006-04-10 18:27:22"
     humandate: "10 Apr, 2006"
     content: | 
       Здесь не большое обсуждение:
       http://xpoint.ru/forums/internet/html_css/css/thread/36200.xhtml

     email: "gordi@kaluga.ru"

  -  author: "Blog: Alter World"
     id: "2954"
     url: "http://astro.physfac.bspu.secna.ru/~aw/blog/2006/04/blog-times-no11.html"
     date: "2006-04-18 07:20:23"
     humandate: "18 Apr, 2006"
     content: | 
       [...] но себе на заметку возьму и выскажу одно замечание по рецепту Простой тултип или всплывающая подсказка – на мой взгляд там нужного результата можно было добиться проще, главное не забывать про DOM и onmouseover/onmouseout.[...]

     email: ""

  -  author: "pepelsbey"
     id: "3161"
     url: "http://pepelsbey.net"
     date: "2006-05-06 15:19:54"
     humandate: "06 May, 2006"
     content: | 
       Битая ссылка на Agat'a "К тому же можно вспомнить о поисковой оптимизации и использовать вот этот прием"
       
       Вот новая: http://agat.in/1/css-seo/

     email: "pepelsbey@gmail.com"

  -  author: "Aph1na"
     id: "3668"
     url: "http://www.otebe.com"
     date: "2006-06-22 15:43:47"
     humandate: "22 Jun, 2006"
     content: | 
       Как-то давно прочитала, но только сегодня пришлось воспользоваться. Огромное спасибо, отличный пример.

     email: "aph1na83@gmail.com"

  -  author: "links for 2006-09-28"
     id: "5287"
     url: "http://andyb.wordpress.com/2006/09/28/links-for-2006-09-28/"
     date: "2006-09-28 05:44:29"
     humandate: "28 Sep, 2006"
     content: | 
       [...] tember 28, 2006  links for 2006-09-28 	Filed under: web andyb 6:23 am 	 		#
       cssing :: Архив :: Простой тултип или всплывающая подсказка
       (tags: webdev css)
       ° [...]

     email: ""

  -  author: "Alex"
     id: "6316"
     url: "http://mauzon.com"
     date: "2006-10-25 23:47:33"
     humandate: "25 Oct, 2006"
     content: | 
       Я думаю, самым корректным и для поисковиков, и для семантики, и для контент-менеджеров будет писать ссылке артибут title, использовать Ваш CSS, а потом javascript'ом для всех A в документе, у которых не пустой title, создать span и положить в него содержимое title'а.
       Скриптик на строк 6, я полагаю :)

     email: "alex@mauzon.com"

  -  author: "akella"
     id: "6329"
     url: "http://cssing.org.ua"
     date: "2006-10-26 19:00:00"
     humandate: "26 Oct, 2006"
     content: | 
       У меня всегда была какая то легкая антипатия к подобным скриптам ) Я фанат простоты и прозрачности. Но отличная идея - это действительно было бы завершенное и <strong>правильное</strong> решение. Спасибо!
       уже не в этот пост но стоит на досуге таки сделать )

     email: "akella.a@gmail.com"

  -  author: "Alex"
     id: "6401"
     url: "http://mauzon.com"
     date: "2006-10-30 00:39:34"
     humandate: "30 Oct, 2006"
     content: | 
       Вот как - оказывается мне не идет мейл об ответе...
       Случайно заметил :)
       Именно как фанат простоты и прозрачности я испытываю огромную симпатию к таким маленьким, простым и прозрачным скриптам :)
       Могу написать.
       Надо будет собраться, да :))

     email: "alex@mauzon.com"

  -  author: "Данила"
     id: "14699"
     url: "http://neoprizma.net/"
     date: "2009-08-10 12:20:11"
     humandate: "10 Aug, 2009"
     content: | 
       ну довольно весомо и ни везде работает, на мой взгляд намного проще можно сделать на js - например как здесь - http://neoprizma.net/2009/08/07/alt/

     email: "darkhero@mail.ru"

  -  author: "Angel7"
     id: "11292"
     url: "http://www.dreamocean.info"
     date: "2007-11-09 09:44:15"
     humandate: "09 Nov, 2007"
     content: | 
       Спасибо, пригодилось!

     email: "mail.angel7@inbox.ru"

  -  author: "Ars"
     id: "11417"
     url: ""
     date: "2007-12-06 11:46:31"
     humandate: "06 Dec, 2007"
     content: | 
       И все таки цсс чудесен если не учитывать, что опера 8.х тупит, в 9.х все отлично. Долго искал подходящий способ тултипицо остановился на цсс варианте. Спасибо

     email: "tipo_ars@mail.ru"

  -  author: "Ars"
     id: "11418"
     url: ""
     date: "2007-12-06 11:52:37"
     humandate: "06 Dec, 2007"
     content: | 
       Хотя вру. Опера тупит :)

     email: "tipo_ars@mail.ru"

  -  author: "akella"
     id: "11420"
     url: "http://cssing.org.ua"
     date: "2007-12-06 13:37:21"
     humandate: "06 Dec, 2007"
     content: | 
       да, для нее второй вариант лучше, там без залипания =)
       Рад что техника вам помогла!

     email: "seijuro@yandex.ru"

  -  author: "Андрей"
     id: "12034"
     url: ""
     date: "2008-03-27 16:54:03"
     humandate: "27 Mar, 2008"
     content: | 
       все работает что называется "чики-пики", т.е. без сучка и задоринки. спасибо автору за дельный совет

     email: "lagutin.andriy@gmail.com"

  -  author: "Михаил"
     id: "12057"
     url: ""
     date: "2008-03-31 09:55:05"
     humandate: "31 Mar, 2008"
     content: | 
       Параллельно с попап-титлом в опере выскакивает ее встроенный титл с ссылкой. Может я чего не понимаю, но такая лажа получается. На мой взгляд, лучше уж проверенным (title="...") методом, чем так.

     email: "m_konnov@list.ru"

  -  author: "akella"
     id: "12058"
     url: "http://cssing.org.ua"
     date: "2008-03-31 11:00:31"
     humandate: "31 Mar, 2008"
     content: | 
       Да, для этого гениального броузера лучше не делать попапы теперь. =)

     email: "akella.a@gmail.com"

  -  author: "Nick"
     id: "12249"
     url: ""
     date: "2008-04-11 06:07:08"
     humandate: "11 Apr, 2008"
     content: | 
       проблема с примером статьи - в файрфоксе Flash-объект ставится выше )= чего то не могу побороть

     email: "xan2005@gmail.com"

  -  author: "akella"
     id: "12251"
     url: "http://cssing.org.ua"
     date: "2008-04-11 09:31:10"
     humandate: "11 Apr, 2008"
     content: | 
       Для позиционирования поверх флеш обьектов нужно указывать им в ХТМЛ параметр wmode="transparent"

     email: "akella.a@gmail.com"

  -  author: "Сандро"
     id: "12314"
     url: ""
     date: "2008-04-22 13:34:11"
     humandate: "22 Apr, 2008"
     content: | 
       #links {position: absolute;}
       #links a {display: block; text-decoration: none;}
       #links a:hover {}
       
       #links a span {display:none;}
       #links a:hover span {display: block; position: absolute; width: 150px; color:#d2d2d2; background:#434343; padding:5px; border:1px solid #999999; margin:10px 0 0 -10px}
        
       
       HTML
       
       
       
       <a href="#" rel="nofollow"><b>ул. Немецкого к...</b>БЛА БЛА БЛА</a>
       
       
       
       
       
       Что бы все это заработало в Опере просто уберите top:-10px и left:40px, а позиционируйте marginОМ и все ок!

     email: "llsandro@mail.ru"

  -  author: "Андрей"
     id: "24669"
     url: "http://sitemaker.x10.bz"
     date: "2011-10-30 15:29:02"
     humandate: "30 Oct, 2011"
     content: | 
       Интересная статья! Кстати если кому интересно есть кросс-браузерный хороший способ на на http://sitemaker.x10.bz/articles.php?id=12

     email: "avanesov.andrey@gmail.com"

layout: "layouts/post.njk"
excerpt: "Довольно часто применяю этот простой прием, но еще о нем не рассказывал. Суть - при  наведении мыши на определнный текст появляется краткое пояснение или расширенная информация  рядом с текстом. <a href=\"http://cssing.org.ua/examples/csstooltip/\">Вот пример</a>(и <a href=\"http://cssing.org.ua/examples/csstooltip/index1.html\">пример для оперы</a> - оговорка одна - тултипы не должны перекрывать другие \"тултипные\" ссылки)."
---

Довольно часто применяю этот простой прием, но еще о нем не рассказывал. Суть - при  наведении мыши на определнный текст появляется краткое пояснение или расширенная информация  рядом с текстом. <a href="http://cssing.org.ua/examples/csstooltip/">Вот пример</a>(и <a href="http://cssing.org.ua/examples/csstooltip/index1.html">пример для оперы</a> - оговорка одна - тултипы не должны перекрывать другие "тултипные" ссылки).<!--more-->
<h3>HTML</h3>
Так как :hover пока в ИЕ к сожалению поддерживается только для элемента a(ссылок) то вынужденный код - такой:
<ol class="code">
<li>&lt;a class="tt" href="#"> Текст ссылки</li>
<li>&lt;span>Пояснение к ссылке &lt;/span></li>
<li>&lt;/a></li>
</ol>
Класс tt просто говорит о том что спан внутри таких ссылок будет отображаться по наведению мышки. Без CSS данная конструкция выглядит вполне логично. К тому же можно вспомнить о поисковой оптимизации и использовать <a href="http://agat.in/1/css-seo/">вот этот прием</a>.
<h3>CSS</h3>
Дело за малым - заставить это все работать :).
Вот такое простое CSS волшебство заставит тултип тултипиться :):
<ol class="code">
<li>a.tt span{</li>
<li class="tab">display:none;<small>/*собственно прячем тултип - пока мышь не наведена*/</small></li>
<li>}</li>
<li>a.tt:hover{</li>
<li class="tab">position:relative;<small>/*Ставим точку отсчета для тултипа внутрь данной ссылки*/</small></li>
<li class="tab">z-index:23;<small>/*это нужно что бы тултип показывался поверх этой и других ссылок*/</small></li>
<li>}</li>
<li>a.tt:hover span{</li>
<li class="tab">display:block;<small>/*показываем тултип при наведении*/</small></li>
<li class="tab">position:absolute;</li>
<li class="tab">top:-10px;</li>
<li class="tab">left:40px;<small>/*три строки для позиции тултипа относительно левого верхнего угла ссылки*/</small></li>
<li class="tab">z-index:22;<small>/*мне 22 + см. выше*/</small></li>
<li class="tab">background:#fafafa;<small>/*фон, что бы было видно тултип*/</small></li>
<li>}</li>
</ol>
Вот собственно и все. Остальное украшательсво. Рабочий пример <a href="http://cssing.org.ua/examples/csstooltip/">минимально приукрашенный</a> + <a href="http://akella.org.ua/pro/ratsystem/">пример из жизни</a> (даты 7 8 9 в календаре).
<h3>Конец</h3>
Вот такой до боли простой приемчик, нередко довольно эффектно выглядящий.
Конечно ему не тягаться с тултипами гоняющимися за курсором мыши. Но и им по простоте с ним не тягаться. :)
<ul>
<li><a href="http://cssing.org.ua/examples/csstooltip/">Мой пример</a></li>
<li><a href="http://cssing.org.ua/pro/ratsystem/index_.html">Из одной из страниц кторые я верстал</a> - навести мышь на 7-8-9 числа календаря</li>
<li><a href="http://www.meyerweb.com/eric/css/edge/popups/demo.html">Почти идентичный по реализации</a> - но другой по внешнему виду прием от Эрика Мейера</li>
</ul>
Авось кому сгодится...
<p class="update">
<img src="http://cssing.org.ua/wp-content/themes/akella/images/upd.gif"> Попап имеет вредное свойство "залипать" в Опере. Точнее это Опера имеет вредное свойство оставлять попап видимым даже после отвода мышки от ссылки. Вредное свойство проявляется далеко не всегда.:-)
</p>
<p class="update" style="height:30px;">
<img src="http://cssing.org.ua/wp-content/themes/akella/images/upd.gif"> <a href="http://cssing.org.ua/examples/csstooltip/index1.html">Вариант для оперы</a>
</p>
