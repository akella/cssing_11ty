---
title: "Прелоад через CSS"
date: "2005-09-27"
humanDate: "27 Sep, 2005"
permalink: "2005/09/27/preload-by-css/"
tags: 
  - "xhtmlcss"
  - "useful"
comments: 
  -  author: "besenok"
     id: "2362"
     url: "http://bsn.kiev.ua"
     date: "2005-09-28 09:36:07"
     humandate: "28 Sep, 2005"
     content: | 
       отлично. структурировать знания в одном месте никогда не помешает, а уж темболее знать несколько способов решить такую проблему - очень неплохо. спасибо, отличная статья! :)

     email: "besenok@gmail.com"

  -  author: "ganges"
     id: "2363"
     url: ""
     date: "2005-09-28 11:11:22"
     humandate: "28 Sep, 2005"
     content: | 
       Спасибо за структуризацию. Почитав этот пост, вдруг понял как я стал далек от Ослов, ужас, так и CSS 3 можно по запарке начать использовать. :)
       
       ИМХО, наиболее эффективный и "безопасный" метод - это метод Pixy
       Прелоад через a:link с перебиванием - для меня новость, еще раз спасибо.

     email: "andrey.stefanenko@gmail.com"

  -  author: "polch"
     id: "2398"
     url: "http://www.tobto.com.ua/"
     date: "2005-10-04 13:49:46"
     humandate: "04 Oct, 2005"
     content: | 
       Мне кажется, что метод с “Дырявой” картинкой наиболее гибок и креативен. Спасибо.

     email: "nebesna@bigmir.net"

  -  author: "Julik"
     id: "2420"
     url: "http://live.julik.nl"
     date: "2005-10-11 16:48:52"
     humandate: "11 Oct, 2005"
     content: | 
       c :link это круто. Но метод Pixy еще очень хорошо применим и без фиксированной ширины. Просто надо сделать _большую_ картинку и (к примеру) поставить иконку кнопки в верхний левый угол, а иконку ролловера в нижний левый. Тогда при "полном" смещении фона еще останется запас на увеличение размера текста или увеличение ширины кнопки

     email: "me@julik.nl"

  -  author: "VoSi"
     id: "2434"
     url: ""
     date: "2005-10-12 15:20:03"
     humandate: "12 Oct, 2005"
     content: | 
       а если с визибилити поиграЦа ?

     email: "vosi@vosi.kiev.ua"

  -  author: "akella"
     id: "2752"
     url: "http://cssing.org.ua"
     date: "2006-01-30 17:58:18"
     humandate: "30 Jan, 2006"
     content: | 
       Дык спроси - отвечу - это ведь не просто забытый репозиторий моих статей - это блог :) а я живой чувак.

     email: "akella.a@gmail.com"

  -  author: "beavja"
     id: "2751"
     url: "http://beavka.narod.ru"
     date: "2006-01-30 17:54:24"
     humandate: "30 Jan, 2006"
     content: | 
       Не нашел тут того что мне надо, но прочитал все равно. И за это спасибо.

     email: "beavka@mail.ru"

  -  author: "akella"
     id: "2754"
     url: "http://cssing.org.ua"
     date: "2006-01-30 18:46:03"
     humandate: "30 Jan, 2006"
     content: | 
       2VoSi:
       К сожалению визибилити мне не помог - не закачивает он (бр.) невидимые картинки

     email: "akella.a@gmail.com"

  -  author: "CGS"
     id: "2760"
     url: "http://www.greenkey.ru/"
     date: "2006-02-07 18:02:39"
     humandate: "07 Feb, 2006"
     content: | 
       Зделал как описано где убираеться flicker эффект для IE.
       И вправду убралось моргание. 
       Но осталась вот такая значит ерунда:
       если делать по этому методу , то у нас получаеться, что есть фон нижний (показываем при наведении), сверху ложиться фон верхний (показываем в нормальном состоянии, и убираем при наведении). Так вот браузер всё равно делает запрос на сервер и грузит (или ещё что) картинку фона верхнего.
       Ни кто не в курсе как от этого избавиться ?

     email: "cgs@newmail.ru"

  -  author: "akella"
     id: "2761"
     url: "http://cssing.org.ua"
     date: "2006-02-07 20:12:33"
     humandate: "07 Feb, 2006"
     content: | 
       я так понял это тоьлко в ИЕ? значок загрузки?
       
       ну это скорее глюк броузера с фоном для ссылок :(

     email: "akella.a@gmail.com"

  -  author: "CGS"
     id: "2762"
     url: "http://www.greenkey.ru/"
     date: "2006-02-08 10:23:29"
     humandate: "08 Feb, 2006"
     content: | 
       Да только в IE.
       Про значёк загрузки не совсем понял ?
       
       Так что, решения пока ни у кого нет ?
       И ещё , с хостингом это как нить может быть связано , если да то как ?

     email: "cgs@newmail.ru"

  -  author: "akella"
     id: "2763"
     url: "http://cssing.org.ua"
     date: "2006-02-08 11:00:01"
     humandate: "08 Feb, 2006"
     content: | 
       покажи пример - ссылку на глючное место - что бы можно было точнее что то сказать...
       
       значок загрузки - это часики около курсора - иногда в ие появляются при наведении на ссылки с фоном...

     email: "akella.a@gmail.com"

  -  author: "CGS"
     id: "2764"
     url: "http://www.greenkey.ru/"
     date: "2006-02-08 12:15:45"
     humandate: "08 Feb, 2006"
     content: | 
       http://www.greenkey.ru
       Самое верхнее меню.

     email: "cgs@newmail.ru"

  -  author: "akella"
     id: "2765"
     url: "http://cssing.org.ua"
     date: "2006-02-09 20:27:58"
     humandate: "09 Feb, 2006"
     content: | 
       я смотрел в ИЕ по моему все отлично. 
       
       Конечно он будет делать запрос - потому что фон этот нужен. Но загружается он <b>до</b> конца загрузки страницы - у меня по крайней мере.

     email: "akella.a@gmail.com"

  -  author: "Sergey"
     id: "2783"
     url: ""
     date: "2006-02-19 15:26:42"
     humandate: "19 Feb, 2006"
     content: | 
       Ни один из примеров не работает..
       Можешь кинуть на мыло реально работающий код?

     email: "sergey.zwezdin@gmail.com"

  -  author: "akella"
     id: "2785"
     url: "http://cssing.org.ua"
     date: "2006-02-19 16:09:07"
     humandate: "19 Feb, 2006"
     content: | 
       Как минимум вариант со смещением позиции фона и изменением цвета фона а не картинки очевидно работают - хоть и другие у меня так и не представилась возможность тестировать. Просто они работают не во всех броузерах одинаково насколько я понял.

     email: "akella.a@gmail.com"

  -  author: "W@D"
     id: "2895"
     url: "http://wadowad.narod.ru"
     date: "2006-03-18 00:21:29"
     humandate: "18 Mar, 2006"
     content: | 
       Я додумался до эффекта "дырявой картинки" сам не знаю каким образом. Но тестил сайт в основном "Оперой" (у которой кэш работает на ура), а IE только на машине и, как следствие, обнаружил дозагрузку картинки только потом. Спасибо за правильное понимание кода. Теперь картинки не подгружаются!
       Спасибо!!!

     email: "wadowad@rambler.ru"

  -  author: "W@D"
     id: "2896"
     url: "http://wadowad.narod.ru"
     date: "2006-03-18 00:32:40"
     humandate: "18 Mar, 2006"
     content: | 
       Как всегда сначала написал потом почитал. Короче проблема дозагрузки с дырявой картинкой решается правильным указанием той части фона, которую следует менять при :hover или :link
       Вот так:
       
       A
       {background: #FFFFFF url(pic/rama_ot.gif);}
       A:hover
       {background-color: #DCDCDC;}
       
       Т.е. color - параметр обязательный!
       А если указать: background: #DCDCDC; то рисунок, даже если он дырявый "затмится" (не будет виден).
       
       Также не поможет сдесь повтор строки с указанием другого фона:
       
       A:hover
       {background: #FFFFFF url(pic/rama_ot.gif);}
       
       Тут картинка всё равно будет подгружаться. Речь идёт о IE. Спасибо за внимание.

     email: "wadowad@rambler.ru"

  -  author: "Костя"
     id: "8146"
     url: "http://site3k.net/"
     date: "2007-02-10 16:04:55"
     humandate: "10 Feb, 2007"
     content: | 
       Если кому интересно, смотрите Ссылки и окна. Внешний вид и внутреннее содержание.(http://webdesign.site3k.net/conjuncture/append/d/links.html) Там описываются различные варианты оформления, предзагрузки и открытия.

     email: "discoveri@narod.ru"

  -  author: "kastorskiy"
     id: "9884"
     url: "http://extreme.lviv.ua/"
     date: "2007-03-21 18:08:51"
     humandate: "21 Mar, 2007"
     content: | 
       Понравился метод с a:link тем, что прелоад и остальное описание ссылок находятся в "одном месте".

     email: "kastorskiy@gmail.com"

  -  author: "kastorskiy"
     id: "9886"
     url: "http://extreme.lviv.ua/"
     date: "2007-03-21 19:05:38"
     humandate: "21 Mar, 2007"
     content: | 
       хм, только кажется метод с a:link не работает...
       или это я криво что-то сделал...

     email: "kastorskiy@gmail.com"

  -  author: "akella"
     id: "9888"
     url: "http://cssing.org.ua"
     date: "2007-03-21 19:53:42"
     humandate: "21 Mar, 2007"
     content: | 
       Они довольно капризны и сильно зависят от структуры ЦСС и прочего окружения. Рекомендую все же применять что то вроде идейного кеширования(последние методы). К сожалению по эффективности пока джаваскрипт далеко впереди ЦСС в этом вопросе =(
       Остается пробовать разные решения, посмотрите например <a href="http://www.maratz.com/blog/archives/2005/06/22/preload-hover-images-in-css/">последний комментарий вот тут</a>

     email: "akella.a@gmail.com"

  -  author: "Виталий"
     id: "18541"
     url: "http://dropbydrop.org.ua/"
     date: "2010-04-09 18:46:12"
     humandate: "09 Apr, 2010"
     content: | 
       Спасибо!

     email: "dropbydrop@ukr.net"

  -  author: "Константин"
     id: "10967"
     url: ""
     date: "2007-06-04 00:43:20"
     humandate: "04 Jun, 2007"
     content: | 
       Поправим еще одну небольшую ошибочку в методе с убиранием фона. Сменим a:hover на а, дабы не смущать читателей... )
       
       a {background: url(”default_img.gif”) no-repeat 0 0;}

     email: "aykroyd@mail.ru"

  -  author: "Константин"
     id: "10968"
     url: ""
     date: "2007-06-04 00:46:04"
     humandate: "04 Jun, 2007"
     content: | 
       Поправим еще одну маленькую ошибочку в методе с убиранием фона. Сменим "a:hover" на "a", дабы не смущать начинающих читателей... )
       
       a {background: url(”default_img.gif”) no-repeat 0 0;}

     email: "aykroyd@mail.ru"

  -  author: "AndroNick"
     id: "10971"
     url: ""
     date: "2007-06-12 13:49:38"
     humandate: "12 Jun, 2007"
     content: | 
       Я лично пользовался JavaScript:
       
       function AddPicture(){
       var p1=new Image(); i.src='my_img1.gif';
       var p2=new Image(); i.src='my_img2.gif';
       }
       
       во всех браузерах работает на ура...

     email: "Andronick.Mail@Gmail.com"

  -  author: "AndroNick"
     id: "10972"
     url: ""
     date: "2007-06-12 13:56:30"
     humandate: "12 Jun, 2007"
     content: | 
       Может и не в тему, но я лично использовал JavaScript:
       
       var p1=new Image();
       p1.src='my_img1.gif';
       var p2=new Image();
       p2.src='my_img2.gif';
       ...
       во всех известных мне браузерах работает на ура..
       рисунки подгружаются один раз а дальше просто:

     email: "AndroNick.Mail@GMail.com"

  -  author: "AndroNick"
     id: "10973"
     url: ""
     date: "2007-06-12 14:01:03"
     humandate: "12 Jun, 2007"
     content: | 
       да блин... вечно обрезается... пишу еще раз:

     email: "AndroNick.Mail@GMail.com"

  -  author: "AndroNick"
     id: "10974"
     url: ""
     date: "2007-06-12 14:11:54"
     humandate: "12 Jun, 2007"
     content: | 
       гы, теперь понял!! забыл теги убрать )) :
       
       IMG src="my_img1.gif" onMouseOver='this.src=p2.src;' onMouseOut='soft.src=soft_n.src;'

     email: "AndroNick.Mail@GMail.com"

  -  author: "strix"
     id: "11077"
     url: "http://www.webreview.org.ua"
     date: "2007-07-09 18:48:42"
     humandate: "09 Jul, 2007"
     content: | 
       спасибо за хорошую статью. 
       Хороший способ написать вначале цсс-файла фильтр:
       html {
        filter: expression(document.execCommand("BackgroundImageCache", false, true));
       }

     email: "strix@inbox.ru"

  -  author: "AleksandrIII"
     id: "11415"
     url: ""
     date: "2007-12-05 17:31:24"
     humandate: "05 Dec, 2007"
     content: | 
       А как сделать, без ява скрипта, замену фона без ссылки или так чтобы ссылка не отображалась?

     email: "sa@mail.ru"

  -  author: "Oleg A"
     id: "12022"
     url: "http://www.anapacapital.ru"
     date: "2008-03-24 21:26:03"
     humandate: "24 Mar, 2008"
     content: | 
       А как подгрузить картинку для предпросмотра в браузер при выборе ее в форме?
       Например: p1.src=’C:/Photo/my_img1.gif’'
       В IE5, IE6 получается, а в остальных (IE7, FireFox, Opera) - нет

     email: "anapacap@ya.ru"

  -  author: "Oleg A"
     id: "12023"
     url: "http://www.anapacapital.ru"
     date: "2008-03-24 21:26:51"
     humandate: "24 Mar, 2008"
     content: | 
       А как подгрузить картинку для предпросмотра в браузер при выборе ее в форме?
       Например: p1.src=’C:/Photo/my_img1.gif’'
       В IE5, IE6 получается, а в остальных (IE7, FireFox, Opera) - нет

     email: "anapacap@ya.ru"

  -  author: "Oleg A"
     id: "12024"
     url: "http://www.anapacapital.ru"
     date: "2008-03-24 21:28:48"
     humandate: "24 Mar, 2008"
     content: | 
       А как подгрузить картинку для предпросмотра в браузер при выборе ее в форме?
       Например: p1.src=’C:/Photo/my_img1.gif’'
       В IE5, IE6 получается, а в остальных (IE7, FireFox, Opera) - нет

     email: "anapacap@ya.ru"

  -  author: "oxyk"
     id: "12060"
     url: ""
     date: "2008-03-31 21:25:43"
     humandate: "31 Mar, 2008"
     content: | 
       что делать с прозрачными пингами??? не могу им фон дать, двигать тоже особо не получится из-за ие6 бага на пинги. 
       и моргает в ие7
       есть идеи какие-нибудь? 
       (переделать их в другой формат не могу - фон под ними с градациями :(((

     email: "oxyk.oxyk@gmail.com"

  -  author: "akella"
     id: "12062"
     url: "http://cssing.org.ua"
     date: "2008-03-31 22:56:31"
     humandate: "31 Mar, 2008"
     content: | 
       6му интернет эксплореру придется обойтись без прелоада. Только и всего.
       Всем остальным броузерам можно сделать полупрозрачные ПНГ и все будет загружаться единовременно.

     email: "akella.a@gmail.com"

  -  author: "евген"
     id: "14332"
     url: "http://zabor.ua"
     date: "2009-04-05 16:55:14"
     humandate: "05 Apr, 2009"
     content: | 
       Статья хорошая.Я вот хочу сделать страничку с наложенными друг на друга блоками div.Идея в том,что бы при наведении на видимую часть блока он всплывал в верх,а в нём информация разная,картинки.Подскажи как сделать.У меня не получилось.

     email: "evgen89@i.ua"

  -  author: "cssing :: Архив :: Применение clip для PNG в ИЕ"
     id: "13320"
     url: "http://cssing.org.ua/2008/10/01/clip-it-baby/"
     date: "2008-10-01 13:07:50"
     humandate: "01 Oct, 2008"
     content: | 
       [...] нам использовать background-position. То есть вся крутость от прелоадов и спрайтов со всякими сдвиганиями фона [...]

     email: ""

  -  author: "kapaev"
     id: "14125"
     url: "http://kapaev.ru"
     date: "2009-02-11 17:15:49"
     humandate: "11 Feb, 2009"
     content: | 
       вобщем поэксперементировал я с вашими способами... все работает, но с мелкими косяками в разных броузерах. т.е. в основном в плорере...
       основной косяк начинается именно с подменой-заменой или дозагрузкой ПНГ...
       в некоторых условиях (в ИЕ) фон или даже картинка не заменяется, а накладывается поверх, и в связи с этим ролловер выглядит крайне плохо...
       
       а еще заметил, что прозрачные области ПНГ не раегируют на маусовер )) - 
       способ описанный тут http://cssing.org.ua/2008/10/01/clip-it-baby/ -

     email: "p.kapaev@mail.ru"

  -  author: "Paul"
     id: "18751"
     url: ""
     date: "2010-07-22 14:31:50"
     humandate: "22 Jul, 2010"
     content: | 
       У меня дилетантский вопрос - а как нужно написать ссылку в HTML коде? Нужно ли загружать свою картинку к ссылке HTML? Спасибо заранее.
       
       З.Ы. Статья - супер)

     email: "paulnovikov@ukr.net"

  -  author: "Flank"
     id: "23451"
     url: "http://svobodakoda.net"
     date: "2011-10-20 08:41:43"
     humandate: "20 Oct, 2011"
     content: | 
       Спасибо, пригодилось! Первые два метода кажутся наиболее дельными. Хотя мне больше нравится прелоад через javascript.

     email: "yalonso@rambler.ru"

layout: "layouts/post.njk"
excerpt: "Структурирую свою информацию - несколько способов избежания страшненьких джаваскриптов делающих прелоад картинок.
"
---

Структурирую свою информацию - несколько способов избежания страшненьких джаваскриптов делающих прелоад картинок.
<!--more-->
<h3>Проблема</h3>
Пускай у нас для какого-то элемента по наведению мыши меняется фоновая картинка, типа такого:
<ol class="code">
<li>a{</li>
<li class="tab">background-image:url(default_img.gif)</li>
<li>}</li>
<li>a:hover{</li>
<li class="tab">background-image:url(hover_img.gif)</li>
<li>}</li>
</ol>
В результате когда страничка (и картинка <strong>default_img.gif</strong>) загрузится и пользователь наведет мышь на ссылку - броузер начнет грузить картинку <strong>hover_img.gif</strong> и пользователь сразу ничего не увидит. А если картинка немаленькая, то и пару секунд ничего видеть не будет. 

Вот для этого и нужен так называемый прелоад, загрузить картинки сразу, что бы пользователь не видел этого мигания. Далее следуют 4 способа избежать мигания.
<h3>1. Метод Pixy</h3>
Идея проста - что бы исключить прелоад нужно... исключить вторую картинку.

Помещаем обе картинки для HOVER и для DEFAULT в одно избражение и по наведению мышки просто меняем позицию фона:
<img height="81" width="138" src="/images/img.gif"  class="right" />
<ol class="code">
<li>a {</li>
<li class="tab">background: url("img.gif") no-repeat <strong>0 0</strong> ;</li>
<li>}</li>
<li>a:hover {</li>
<li class="tab">background-position: <strong>0 -40px</strong>;</li>
<li>}</li>
<li>a:active, a#here {</li>
<li class="tab">background-position: <strong>0 -80px</strong>;</li>
<li>}</li>
</ol>
Конечно, это означает фиксированую высоту (или ширину) блока для которого мы делаем этот фон. Иначе фоны бы отображались более одного за раз, или еще как-нить криво.

ИЕ однако и тут выпендрился и решил что так как фон меняется, то надо че то дозагружать. Это так называемый <strong>flicker эффект</strong> - метод борьбы с ним прост - но не всегда реализуем - нужно задать фон для внешнего блока - и тогда ховер эффект реализовывать не смещением позиции фона - а просто его убиранием.
Таким образом в ИЕ можно избавиться от мигания и "дозагрузок" картинок.

Примерно так:
<ol class="code">
<li>#outer{</li>
<li class="tab">background: url("hover_img.gif") no-repeat 0 0;</li>
<li>}</li>
<li>a{</li>
<li class="tab">background: url("default_img.gif") no-repeat 0 0;</li>
<li>}</li>
<li>a:hover {</li>
<li class="tab">background: none;</li>
<li>}</li>
</ol>
<ul>
<li><a href="http://wellstyled.com/css-nopreload-rollovers.html">Оригинальная статья</a> обратите внимание на Update внизу - к вопросу о мигании в ИЕ6</li>
</ul>

<h3>2. Прелоад через a:link</h3>
Таким образом можно закэшировать <strong>hover_img.gif</strong>  для элемента навигации.
Селектор <strong>a:link</strong> "перебивает" просто <strong>a</strong> - поэтому визуально ничего не изменится, но броузер поместит файл в кэш:
<ol class="code">
<li>a{</li>
<li class="tab">background-image: url("hover_img.gif");</li>
<li>}</li>
<li>a:link,a:visited{</li>
<li class="tab">background-image: url("default_img.gif");</li>
<li>}</li>
<li>a:hover{</li>
<li class="tab">background-image: url("hover_img.gif");</li>
<li>}</li>
</ol>
Этот метод в принципе похож на четвертый, но для полноты я описал их отдельно.
<ul>
<li><a href="http://www.maratz.com/blog/archives/2005/06/22/preload-hover-images-in-css/">Preload :hover images in CSS</a></li>
</ul>
<h3>3. "Дырявая" картинка</h3>
Суть такова - в качестве фоновой картинки берем "дырявую", то есть ГИФ с прозрачными областями. А собственно :hover эффект делаем сменой фонового цвета, а не картинки. Однако нам придется фиксировать высоту и ширину элемента, да и сам эффект будет состоять лишь в смене цвета определенной области - но тем не менее:
<ol class="code">
<li>a {</li>
<li class="tab">background:#ccc url("img.gif") no-repeat 0 0;</li>
<li>}</li>
<li>a:hover {</li>
<li class="tab">background-color:#c00;</li>
<li>{</li>
</ol>
Впервые столь простую идею увидел на Simplebits с год-два назад - сейчас уже не смог найти линк.

К примеру:  все следующие изображения сделаны с помощью одной и той же картинки - лишь сменой фонового цвета: <img src="/images/issue.gif" width="13" height="13" alt="*" style="background:#000; padding:0;border:none;" />, <img src="/images/issue.gif" width="13" height="13" alt="*" style="background:#c00;padding:0;border:none;" />, <img src="/images/issue.gif" width="13" height="13" alt="*" style="background:#00c;padding:0;border:none;" />, <img src="/images/issue.gif" width="13" height="13" alt="*" style="background:#0c0;padding:0;border:none;" />. Фоновый цвет "светит" через прозрачные дыры в картинке. Сама же картинка лишь белого цвета.

Идею можно применять не только для  :hover эффектов, но и для многоразового юзания одной картинки в разных цветах.
<h3>4. Прелоад через указание фона для чего-нибудь</h3>
Можно поместить картинку для :hover в кэш браузера путем таких вот махинаций:
<ol class="code">
<li>h2 {</li>
<li class="tab">background:url("hover_img.gif') no-repeat;</li>
<li class="tab">background-position:-1000px -1000px;</li>
<li>}</li>
</ol>
Отличается от номера 2 только тем, что тут фон прячут позицией, а не "перебиванием" более сильным селектором.
<ul>
<li><a href="http://www.paulpgriffin.com/css/tabs/tabs.html">Подсмотрено тут</a></li>
</ul>
<h3>В конце</h3>
Все здесь описанное не претендует на оригинальность - скорее структурирую свои же знания - да и вдруг кому-то это окажется полезным. Почти все приемы просты до безобразия. Но в этом вся соль.

Как говорил один человек - я горжусь тем, что так много "украл" у других. :)

Кто знает еще какие-то способы - пишите в комменты. Думаю от этого выиграем мы все.
