---
title: "Слайсы на kremlin.ru"
date: "2010-03-12"
humanDate: "12 Mar, 2010"
permalink: "2010/03/12/kremlin-slice/"
tags: 
  - "xhtmlcss"
  - "web-standards"
comments: 
  -  author: "Samter"
     id: "18478"
     url: "http://ebrest.by/"
     date: "2010-03-27 06:57:29"
     humandate: "27 Mar, 2010"
     content: | 
       Полезная информация. Никогда раньше не пользовался этими слайсами.
       Еще раз спасибо.

     email: "denis@rudov.com"

  -  author: "Del'ka"
     id: "18557"
     url: "http://delka.name"
     date: "2010-04-15 13:56:09"
     humandate: "15 Apr, 2010"
     content: | 
       К слайсу применяются не только инлайновые стили, но и стили прописанные в css исключительно для слайса.
       
       Чтобы задать разные стили для слайса и его вида внутри страницы я делал так:
       
       Допустим слайс у нас лежит в div.content
       
       
       
       
       
       в css:
       slice {стили применяемые только к слайсу}
       div.content slice {стили применяемые к слайсу на странице, они перебивают стили просто слайса}

     email: "delka@anime.kharkov.ua"

  -  author: "akella"
     id: "18537"
     url: "http://cssing.org.ua"
     date: "2010-04-08 13:44:18"
     humandate: "08 Apr, 2010"
     content: | 
       Точно, они сами на msdn говорят что это очень похоже на iframe. Все что угодно в этом окошке. И сам слайс <a href="http://kremlin.ru/slice/news" rel="nofollow">отдельная полноценная страничка</a> со своим доктайпом и прочим

     email: "akella.a@gmail.com"

  -  author: "Чистяков Денис"
     id: "18536"
     url: ""
     date: "2010-04-08 13:17:13"
     humandate: "08 Apr, 2010"
     content: | 
       Спасибо за полезный и доходчивый обзор, как простая, приятная и удобная мелочь на сайте -- самое оно.
       Я правильно понимаю, что туда можно и поисковую форму поместить например, если поиск востребован, или какой то фильтр для каталога?
       В том плане что это получается полноценная HTML страница отрендеренная IE, да?

     email: "den.chistyakov@gmail.com"

  -  author: "Heller"
     id: "17342"
     url: "http://www.okburo.ru"
     date: "2010-03-12 15:11:35"
     humandate: "12 Mar, 2010"
     content: | 
       К вопросу "а зачем?":
       На портал приходит значительная доля ie8, по объективным причинам.

     email: "darkboutique@gmail.com"

  -  author: "Toxa"
     id: "17374"
     url: ""
     date: "2010-03-13 10:56:35"
     humandate: "13 Mar, 2010"
     content: | 
       Отлично описано! Очень полезная фишка!

     email: "grand_toxa@mail.ru"

  -  author: "Александр"
     id: "17372"
     url: "http://www.delaform.ru"
     date: "2010-03-12 20:45:11"
     humandate: "12 Mar, 2010"
     content: | 
       Главное чтобы людям было удобно.

     email: "symbio@ya.ru"

  -  author: "progg.ru"
     id: "17371"
     url: "http://progg.ru/%D0%A1%D0%BB%D0%B0%D0%B9%D1%81%D1%8B-%D0%BD%D0%B0-kremlinru"
     date: "2010-03-12 19:57:20"
     humandate: "12 Mar, 2010"
     content: | 
       <strong>Слайсы на kremlin.ru...</strong>
       
       Trackback from progg.ru...

     email: ""

  -  author: "akella"
     id: "17357"
     url: "http://cssing.org.ua"
     date: "2010-03-12 16:44:37"
     humandate: "12 Mar, 2010"
     content: | 
       Да, я работаю над этим сайтом в составе &laquo;<a href="http://www.okburo.ru/" rel="nofollow">Опытного Креативного Бюро</a>&raquo;

     email: "akella.a@gmail.com"

  -  author: "Никита"
     id: "17354"
     url: ""
     date: "2010-03-12 16:25:06"
     humandate: "12 Mar, 2010"
     content: | 
       Ты сайт медведеву верстаешь ?

     email: "nikit@mail.ua"

  -  author: "ArtemChertov"
     id: "17530"
     url: "http://artem.chertov.name"
     date: "2010-03-15 14:41:35"
     humandate: "15 Mar, 2010"
     content: | 
       Интересно! Пока не приходилось сталкиваться.
       Спасибо, Юр :)

     email: "artem@chertov.name"

  -  author: "inst"
     id: "41511"
     url: "http://www.inst.tk/"
     date: "2012-02-22 22:47:46"
     humandate: "22 Feb, 2012"
     content: | 
       Расскажите, пожалуйста, как это работает в IE9?
       Так сказать, два года спустя.

     email: "inst@gmx.com"

layout: "layouts/post.njk"
excerpt: "Сегодня запустили слайсы на kremlin.ru. Небольшой рассказ чтобы упростить внедрение в будущем.
"
---

Сегодня запустили слайсы на kremlin.ru. Небольшой рассказ чтобы упростить внедрение в будущем.
<!--more-->
<h3>Что это вообще такое эти слайсы?</h3>
Это что-то вроде продвинутых закладок для IE8.  Вы можете выбрать кусочек страницы, добавить его в Favorites. И после этого находясь уже на другом сайте, просмотреть этот кусочек. По клику на закладку откроется небольшое окошко с фрагментом другой страницы. Например это может быть погода, вот так это выглядит в слайсе от gismeteo:
<p class="img"><img src="http://cssing.org.ua/pic/slices/gismeteo.png" alt=""  width="458" height="379"><span>Заметьте, что при этом я нахожусь на сайте Digg</span></p>
Или это может быть десятка популярных линков Digg:
<p class="img"><img src="http://cssing.org.ua/pic/slices/digg.png" alt=""  width="458" height="379"><span>А теперь я на gismeteo, но держу руку на пульсе Digg! Я непредсказуем - согласитесь.</span></p>
Идея в том, что вам не нужно заходить на сайт, можно загрузить только тот кусочек который важен. 
Но, обновлять так можно не любой фрагмент сайта, а только отдельные, предусмотренные сайтом. Фрагменты подсвечиваются примерно так:
<p class="img"><a href="http://cssing.org.ua/pic/slices/kremlin.jpg"><img src="http://cssing.org.ua/pic/slices/kremlin_small.png" alt=""  width="460" height="279"><span>Картинка кликабельна</span></a></p>
Такая вот полезная мелочь. А для больших сайтов, как известно, все мелочи значимы. 
<h3>Что это такое для кодера</h3>
Не более чем набор микроформатов (за нас придуманных названий классов). Ничтоже сумняшеся перейдем к коду, он очень прост:
<ol class="code">
<li>&lt;div <strong>class=&quot;hslice&quot; id=&quot;whatever&quot;</strong>&gt;</li>
<li class="tab">&lt;div <strong>class=&quot;entry-title&quot;</strong>&gt;Название слайса.&lt;/div&gt;</li>
<li class="tab">&lt;div <strong>class=&quot;entry-content&quot;</strong>&gt;А тут то что будет отображаться в окошке слайса.&lt;/div&gt;</li>
<li>&lt;/div&gt;</li>
</ol>
Пару классов, и какой-то, любой, но заданный id.
Это пример самого элементарного слайса.
В моем случае было что-то вроде этого:
<ol class="code">
<li>&lt;div class=&quot;b-news-main <strong>hslice</strong>&quot; id=&quot;news&quot;&gt;</li>
<li class="tab">&lt;h2 <strong>class=&quot;entry-title&quot;</strong>&gt;Новости&lt;/div&gt;</li>
<li class="tab">&lt;ul class="entry-content"&gt;<small>...список новостей...</small> &lt;/ul&gt;</li>
<li>&lt;/div&gt;</li>
</ol>
Это код с <a href="http://kremlin.ru">главной</a>. А результат получился такой:
<p class="img"><img src="http://cssing.org.ua/pic/slices/fail.png" alt=""  width="396" height="285"><span>Очень мило</span></p>
Неприятные мысли стали посещать меня в этот момент.
Но я снова воспрял духом едва прочитал документацию до конца. Оказалось, из стилей наложенных на этот фрагмент на оригинальной странице, берутся только инлайновые, и никаких наследованных  (<code>body{font-size:12px}</code> не применяется).

<code>style="font-size:12px;"</code> применился бы, но кому интересно марать свой чистый код.
<h3>Правильный путь</h3>
Можно, и я думаю нужно, подключать контент для слайса из отдельного файла. Какова бы ни была ваша страница, стили наложенные на фрагмент <em>на сайте</em>, вряд ли красиво переложатся в это <em>маленькое окошко</em> слайса в браузере.

В <a href="http://msdn.microsoft.com/library/cc848871(VS.85).aspx">документации</a> описано несколько путей. Нам подошел следующий.
Код на сайте:
<ol class="code">
<li>&lt;div class=&quot;b-news-main hslice&quot; id=&quot;news-slice&quot;&gt;</li>
<li class="tab">        &lt;h3 class=&quot;entry-title&quot;&gt;Новости&lt;/h3&gt;</li>
<li class="tab"><strong>&lt;a rel=&quot;feedurl&quot; href=&quot;/slice/news&quot;&gt;&lt;/a&gt;</strong></li>
<li class="tab">...</li>
<li>&lt;/div&gt;
</ol>
Параметр feedurl используется для указания альтернативного источника для слайса, как раз то что нам нужно в данном случае.

А по адресу <a href="http://kremlin.ru/slice/news">/slice/news</a> находится файл который я хочу чтобы отображался в браузере.

При этом важно помнить, что внутри этого файла снова должен быть размечен слайс, поскольку IE рассматривает его именно как <em>альтернативный источник</em>, который снова надо парсить. Если просто вставить в этом файле какой-либо HTML (было бы логично) слайс не будет работать в браузере. <a href="http://kremlin.ru/slice/news">Вот такое там содержимое прямо сейчас</a>:
<ol class="code">
<li>&lt;div class=&quot;hslice entry-content&quot; id=&quot;documents&quot;&gt;</li>
<li class="tab">&lt;h2 class=&quot;entry-title&quot;&gt;Новости&lt;/h2&gt;</li>
<li class="tab"><small>&lt;!--Адрес куда IE будет ходить при обновлении, сюда же --&gt;</small></li>
<li class="tab">&lt;a rel=&quot;entry-content&quot; href=&quot;http://news.kremlin.ru/slice/news&quot; style=&quot;display: none;&quot; &gt;&lt;/a&gt;</li>
<li class="tab">&lt;ul class=&quot;entry-content&quot;&gt;</li>
<li class="tabtab"><small>список новостей</small></li>
<li class="tab">&lt;/ul&gt;</li>
<li>&lt;/div&gt;</li>
</ol>
Как видно, обычный слайс с которого мы начинали. И теперь наконец все работает! На этом мы пока и остановились. Слайс в действии можно видеть <a href="http://kremlin.ru">на этой страничке</a>, а файл самого слайса <a href="http://kremlin.ru/slice/news">берется отсюда</a>.
Выглядит это прямо сейчас вот так:
<p class="img"><img src="http://cssing.org.ua/pic/slices/result.png" alt=""  width="460" height="382"><span>Слайс можно растянуть по вертикали чтобы уместилось больше новостей</span></p>
А вот так распознается браузером:
<p class="img"><img src="http://cssing.org.ua/pic/slices/result1.png" alt=""  width="527" height="229"></p>
После, я еще много игрался и комбинировал эти методы, если кому-то интересно, вы тоже можете окунуться с головой в увлекательный мир слайсов под IE8. Но я решил удовлетвориться одним рабочим вариантом :)


<h3>Ссылки</h3>
<ul>
<li><a href="http://habrahabr.ru/blogs/ie/72189/">Подробная статья на Хабрахабре</a></li>
<li><a href="http://msdn.microsoft.com/library/cc848871(VS.85).aspx">Про слайсы на MSDN</a></li>
<li><a href="http://ieaddons.com/ru/webslices/">Слайсы на других русскоязычных сайтах</a></li>
</ul>

Надеюсь кому-то это сэкономит время в будущем, и буду рад вашему опыту! 
В одном из следующих постов могу рассказать об опыте вёрстки этого большого проекта. И почему все получилось сделать валидным.

P.S.: Так как у меня windows XP, и в ней стоит родной IE6, который я не хотел терять, тестировал я все в <a href="http://ru.wikipedia.org/wiki/Software_as_a_service">SaaS</a> решении <a href="http://spoon.net/">Spoon.net</a>. Нужно лишь установить плагин порядка 25 мегабайт, и можно запускать почти <a href="http://spoon.net/browsers/">любой браузер</a> (всё это работает правда пока под Windows).
