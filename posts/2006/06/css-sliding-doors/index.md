---
title: "Идея раздвижных дверей в CSS"
date: "2006-06-08"
humanDate: "08 Jun, 2006"
permalink: "2006/06/08/css-sliding-doors/"
tags: 
  - "xhtmlcss"
comments: 
  -  author: "Flack"
     id: "3513"
     url: "http://flack.ru"
     date: "2006-06-08 17:09:24"
     humandate: "08 Jun, 2006"
     content: | 
       При увеличении шрифта ужасы происходят :)

     email: "alex@flack.ru"

  -  author: "akella"
     id: "3514"
     url: "http://cssing.org.ua"
     date: "2006-06-08 17:20:53"
     humandate: "08 Jun, 2006"
     content: | 
       В курсе ( больше года назад как верстал... Но...
       Лень, диплом, лето, руководство, для которого это не приоритет..... так что не казни сразу, когда-нибудь все будет Elastic ;)
       PS Мне все равно стыдно.

     email: "akella.a@gmail.com"

  -  author: "ZeT"
     id: "3515"
     url: ""
     date: "2006-06-08 19:47:29"
     humandate: "08 Jun, 2006"
     content: | 
       такой приём не очень работает, если у фона вырезаны углы с прозрачностью...

     email: "zet@frogler.ru"

  -  author: "akella"
     id: "3516"
     url: "http://cssing.org.ua"
     date: "2006-06-09 00:16:14"
     humandate: "09 Jun, 2006"
     content: | 
       Это не совсем правильно. Просто он чуть чуть усложняется.
       Второй пример с вертикальными раздвижными дверями как раз с прозрачными углами. И, насколько видно, прием работает.
       
       Если бы в данном случае картинка была с прозрачным углами достаточно было бы исправить для фона:
       <ol class="code">
       <li>#searchrow form{</li>
       <li class="tab">background: <del>transparent</del> #fff url(pic/bg_search.gif) no-repeat 0 0;</li>
       </ol>
       И все было бы как надо. 
       Если же там обязательно был нужен какой то градиентный просвечивающий фон(кстати во втором <a href="http://cssing.org.ua/examples/sliding/" rel="nofollow">примере</a> именно так, в ФФ) то пришлось бы еще покумекать. Но целью я ставил показать идею, а не сделать супер универсальное решение одной желтой картинкой всё-всё-всё :)
       А по большому счету, просто сказать что мне эта идея нравится.
       
       Наверно в случае мегаважной прозрачности для этой желтой картинки было бы удобнее как то по-другому порезать её. Панацей не существует.

     email: "akella.a@gmail.com"

  -  author: "ganges"
     id: "3523"
     url: ""
     date: "2006-06-09 15:11:52"
     humandate: "09 Jun, 2006"
     content: | 
       Хороша идея и очень доходчиво ты ее объясняешь. Я, например находился в плену парадигмы ul li для этой идеи :) а теперь очевидная вещь стала понятна как гром среди ясного неба. 
       А насчет прозрачности так это сами знаете почему отнюдь не универсальная вещь, надо будет iepngtransparencyfix.js писать еще :)

     email: "andrey.stefanenko@gmail.com"

  -  author: "Setti @ PlayStation"
     id: "3901"
     url: "http://playstation-blog.ru/"
     date: "2006-07-14 17:32:05"
     humandate: "14 Jul, 2006"
     content: | 
       А почему не использовал скругленные углы без использования изображений?

     email: "setti@setti.biz"

  -  author: "akella"
     id: "4444"
     url: "http://cssing.org.ua"
     date: "2006-08-18 12:35:55"
     humandate: "18 Aug, 2006"
     content: | 
       Для скругления используются несколько дивов - угол на смом деле не круглый, но расположение дивов создает попиксельную иллюзию того что он круглый.
       Здесь подробнее - http://www.html.it/articoli/nifty/index.html

     email: "akella.a@gmail.com"

  -  author: "Merle"
     id: "4437"
     url: "http://www.greenkey.ru"
     date: "2006-08-18 09:31:38"
     humandate: "18 Aug, 2006"
     content: | 
       Скругленные углы без изображений - это вы что имеете ввиду?

     email: "web@greenkey.u"

  -  author: "akella"
     id: "4503"
     url: "http://cssing.org.ua"
     date: "2006-08-20 15:44:01"
     humandate: "20 Aug, 2006"
     content: | 
       Почти все книги хороши для начала, хотя много информации сосредоточено например на alistpart.com и у многих зарубежных блоггеров. Книга Зельдмана "Designiing With Web Standards"(<a href="http://www.ozon.ru/context/detail/id/2369681/" rel="nofollow">на русском</a>) совсем не плоха, остальные современные книги в основном еще не переведены. <a href="http://simplebits.com/publications/" rel="nofollow">Книги Дэна Цедерхолма</a> тоже были бы очень полезны для прочтения.

     email: "akella.a@gmail.com"

  -  author: "ShmaToK"
     id: "4502"
     url: "http://pulya.net"
     date: "2006-08-20 15:16:57"
     humandate: "20 Aug, 2006"
     content: | 
       А кто-то вообще может подсказать книгу по css?

     email: "shmatoks@pulya.net"

  -  author: "Zigzag"
     id: "4569"
     url: "http://lovata.com"
     date: "2006-08-24 13:10:51"
     humandate: "24 Aug, 2006"
     content: | 
       Кстати, тот самый Седерхольм в своей книге "Пуленепробиваемый вебдизайн" описывает технику создания растягивания подобного бокса как по вертикали, так и по горизонтали одновременно + еще и шрифт задан не в пикселях. Вот пример, если кому интересно:
       
       
       
       
       
       
       
       @import url("style.css"); 
       
       
       
       
       This box is:
       	<em><a href="/browsers/firefox/" rel="nofollow">Indestructible!</a></em>	
       
       
       
       
       
       .container {
       	float: left;
       	color: #666;
       	background: url(images/rounded-right.gif) no-repeat top right;
       }
       .desc {
       	margin: 0;
       	padding: 9px 9px 0 9px;
       	background: url(images/rounded-left.gif) no-repeat top left;
       }
       .link {
       	margin: 0;
       	padding: 0 0 0 9px;
       	background: url(images/rounded-left.gif) no-repeat bottom left;	
       }
       .link em {
       	display: block;
       	padding: 0 9px 9px 0;
       	font-style: normal;
       	background: url(images/rounded-right.gif) no-repeat bottom right;	
       }
       .container a {
       	font-size: 130%;
       	color: #E70;
       }
       
       изображения:
       
       1.rounded-left.gif 9х200 (WxH)
       2.rounded-right.gif 400x200

     email: "zigzag85@mail.ru"

  -  author: "Zigzag"
     id: "4570"
     url: "http://lovata.com"
     date: "2006-08-24 13:11:53"
     humandate: "24 Aug, 2006"
     content: | 
       не понял, почему вместо xhtml кода вывелось
       
       @import url(”style.css”);
       
       This box is:
       Indestructible! 
       
       ???

     email: "zigzag85@mail.ru"

  -  author: "0lympian"
     id: "5630"
     url: ""
     date: "2006-10-13 14:10:59"
     humandate: "13 Oct, 2006"
     content: | 
       Ну... на самом деле это вариация на тему четырех вложенных дивов с прижатыми "уголками" для каждого из них. Ну и маргин для текста внутри него.

     email: "0lympy@gmail.com"

  -  author: "akella"
     id: "55602"
     url: "http://cssing.org.ua"
     date: "2012-05-14 21:25:09"
     humandate: "14 May, 2012"
     content: | 
       Нужно просто взять такую же картинку но намного бОльшего чем нужно размера - все остальные техники остаются такими же.

     email: "akella.a@gmail.com"

  -  author: "Denys"
     id: "55599"
     url: ""
     date: "2012-05-14 20:29:10"
     humandate: "14 May, 2012"
     content: | 
       Огромное спасибо за статью, все написано ясно и понятно! Но у меня закрался вопрос:как сделать такой блок резиновым? Например: делаем резиновую верстку с условием, что в ряд идут несколько блоков фиксированной ширины, а последний блок должен занимать все оставшееся пространство. Ширина контента внутри не меняется.
       Буду очень признателен за ответ

     email: "d.kolesnychenko@gmail.com"

layout: "layouts/post.njk"
excerpt: "Наверное одна из первых статей про CSS, которая меня захватила, была \"<a href=\"http://www.id-as.com/arts/ala/slidingdoors/\">Раздвижные двери CSS</a>\" (<a href=\"http://www.id-as.com/arts/ala/slidingdoors2/\">и вторая часть</a>)(<a href=\"www.alistapart.com/articles/slidingdoors/\">оригинал</a>). Мне понравилось, что для решения некоторых проблем верстки порой нужно хоть и чуть-чуть, но нестандартно мыслить. В результате эта идея(раздвижных дверей) несколько раз сэкономила мне время. Вот пара применений, из которых Вы, я надеюсь, уловите идею и может быть она кому то поможет. И хотя многие наверняка знакомы с ней, тем не менее..."
---

Наверное одна из первых статей про CSS, которая меня захватила, была "<a href="http://www.id-as.com/arts/ala/slidingdoors/">Раздвижные двери CSS</a>" (<a href="http://www.id-as.com/arts/ala/slidingdoors2/">и вторая часть</a>)(<a href="www.alistapart.com/articles/slidingdoors/">оригинал</a>). Мне понравилось, что для решения некоторых проблем верстки порой нужно хоть и чуть-чуть, но нестандартно мыслить. В результате эта идея(раздвижных дверей) несколько раз сэкономила мне время. Вот пара применений, из которых Вы, я надеюсь, уловите идею и может быть она кому то поможет. И хотя многие наверняка знакомы с ней, тем не менее...<!--more-->
<h3>Раздвижные двери на ukr.net</h3>
Когда то давно на сайте укр.нет, еще когда я его первый раз переделывал (<a href="http://cssing.org.ua/examples/ukrnet/">вот тут вариант</a>) была желтая область для поиска, она задавалась в фоне одной картинкой - <a href="http://cssing.org.ua/examples/ukrnet/pic/bg_search.gif">вот такой вот большой</a> и выглядело вот так:
<img src="/images/ukrnet-2.png">
Однако позднее понадобился редизайн, где эта область начинала занимать две трети колонки. А сейчас она вообще в ширину средней колонки - <a href="http://www.ukr.net/">сами посмотрите</a>:
<img src="/images/ukrnet-1.png">
Естественно, когда запахло первым изменением ее ширины мне было лень перерисовывать картинку в нужную ширину. Конечно захотелось сделать это как то более ширино-независимо.(наверно, потому что я знал, что ее ширина еще 10 раз изменится). На помощь пришли "раздвижные двери".
Итак, задача:<strong> была область широкая с одной фоновой картинкой. Как, не перерисовывая картинку, сделать область уже, и тоже с круглыми краями?</strong>
Вот такой там был код HTML(и сейчас такой):
<ol class="code">
<li>&lt;!-- #searchrow --&gt;</li>
<li>&lt;div id=&quot;searchrow&quot;&gt;</li>
<li class="tab">&lt;form &gt;</li>
<li class="tab">...</li>
<li class="tab">&lt;/form&gt;</li>
<li>&lt;/div&gt;</li>
<li>&lt;!--END #searchrow --&gt;</li>
</ol>
Для начала зададим этот фон(большой который) для внешнего дива:
<ol class="code">
<li>#searchrow{</li>
<li class="tab">height:60px;</li>
<li class="tab">background: #fff url(pic/bg_search.gif) no-repeat 100% 0;</li>
</ol>
Вот что выйдет:
<img src="/images/ukrnet-3.png" />
Слева край не круглый.
Тогда добавим  еще для формы:
<ol class="code">
<li>#searchrow form{</li>
<li class="tab">height:60px;<small>/*для одинаковой высоты*/</small></li>
<li class="tab">background: transparent url(pic/bg_search.gif) no-repeat 0 0;</li>
</ol>
Получим вот что:
<img src="/images/ukrnet-5.png" />
Сейчас у нас две картинки фоновых - одна поверх другой. Осталось раздвинуть двери:
<ol class="code">
<li>#searchrow {</li>
<li class="tab">padding-right:10px;</li>
</ol>
В результате:
<img src="/images/ukrnet-6.png" />
То что нужно. Блок формы (#searchrow form) отодвинулся:
<img src="/images/ukrnet-8.png" />
И если вы не умея рисовать в Фотошопе попробуете это изобразить для своего поста на блоге (что бы <strong>всем</strong> стало понятно), то выйдет(заодно прокляв маленькую ширину контент-области на блоге :)):
<img src="/images/ukrnet-7.gif" />
(<a href="http://cssing.org.ua/images/ukrnet-4.png">а здесь чуть больше</a>)
Если попытаться представить себе это то - мы как бы отодвинули одну дверку - из-за которой стал светить нижний фон.
Вот таким вот образом с помощью все той же большой картинки получилось сделать желтую область с круглыми краями для произвольной длины блока - ограниченной конечно шириной большой желтой картинки.

Может из-за многословности(многокартинковости) красота идеи немного смазалась - но оглянитесь, 3-4 строчки ЦСС сэкономили нам открытие фотошопа. Мне кажется это немало.
<h3>Вообще</h3>
Вообще же очевидно что присобачить эту идею(как и любую хорошую идею) можно к чему угодно. Раздвигать двери можно и по вертикали. <a href="http://cssing.org.ua/examples/sliding/">Вот тут</a> например я их развиднул по вертикали.(опять же для круглых краев, красным и зеленым обозначены "двери")
Стоит вспомнить оригинальную статью Дага Баумана где он их раздвигал для навигации. Для ее(идеи) применения достаточно ее прочувствовать, сделать своей, или украсть как я это называю. :)
Впрочем не такая она сложная, и я уверен что многие ее с успехом применяли, но надеюсь кому то это все же поможет.
<h3>Ссылки по этой теме</h3>
Пытался быть максимально понятным, но вот еще информация по этой теме:
<ul>
<li><a href="http://www.alistapart.com/articles/slidingdoors/">Sliding Doors of CSS</a> (<a href="http://www.alistapart.com/articles/slidingdoors2/">part 2</a>) - оригинальная статья Дага Баумана</li>
<li><a href="http://www.id-as.com/arts/ala/slidingdoors/">Раздвижные двери CSS</a> (и <a href="http://www.id-as.com/arts/ala/slidingdoors2/">вторая часть</a>) - переводы Андрея Смирнова</li>
</ul>
