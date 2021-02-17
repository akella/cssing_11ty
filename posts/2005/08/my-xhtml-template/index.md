---
title: "HTML заготовки"
date: "2005-08-24"
humanDate: "24 Aug, 2005"
permalink: "2005/08/24/my-xhtml-template/"
tags: 
  - "xhtmlcss"
  - "useful"
comments: 
  -  author: "agat"
     id: "2099"
     url: "http://cssdesign.ru"
     date: "2005-08-24 14:47:28"
     humandate: "24 Aug, 2005"
     content: | 
       А, у меня xtml заготовка вот такая:
       <ol class="code">
       <li>&lt;!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/
       xhtml1-transitional.dtd"&gt;</li>
       <li>&lt;html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en"&gt;</li>
       <li>&lt;head&gt;</li>
       <li class="tab">&lt;meta http-equiv="Content-Type" content="text/html; charset=windows-1251" /&gt;</li>
       <li class="tab">&lt;title&gt;seo&lt;/title&gt;</li>
       <li class="tab">&lt;link rel="stylesheet" href="styles.css" type="text/css" /&gt;</li>
       <li>&lt;/head&gt;</li>
       <li>&lt;body&gt;</li>
       <li>&lt;div id="site"&gt;</li>
       <li class="tab">&lt;div id="header"&gt;</li>
       <li class="tab">&lt;/div&gt;</li>
       <li class="tab">&lt;div id="menu"&gt;</li>
       <li class="tab">&lt;/div&gt;</li>
       <li class="tab">&lt;div id="content"&gt;</li>
       <li class="tab">&lt;/div&gt;</li>
       <li class="tab">&lt;div id="footer"&gt;</li>
       <li class="tab">&lt;/div&gt;</li>
       <li>&lt;/div&gt;</li>
       <li>&lt;/body&gt;</li>
       <li>&lt;/html&gt;</li>
       </ol>
       
       
       
       
       
       
       	
       	
       	
       	
       	
       	
       	
       		
       	
       	
       	
       
       	
       	
       	
       
       
       
       
       </code>

     email: "tindery@yandex.ru"

  -  author: "ganges"
     id: "2101"
     url: ""
     date: "2005-08-24 15:29:48"
     humandate: "24 Aug, 2005"
     content: | 
       Привет, Акелла!
       
       meta name=&#8221;robots&#8221; content=&#8221;all, index, follow&#8221;
       
       Вот я долго думал когда-то над своими CSS файлами, что же входит в "понятие" base.css?
       Для меня master.css это screen.css по аналогии c print.css и handheld.css
       
       screen.css импортирует:
       
       layout.css (видимо для меня лэйаут это и есть тот бэйс)
       
       textformatting.css (размеры, семьи, отступы)
       
       hacks.css (всю байду для ослов очень удобно вписать сюда, в отдельный файл, как советуют отцы и матери, на тот случай, если семерка приподнесет какие-то реальные новшества, в чем лично я сильно сомневаюсь)
       
       и... visuals.css ( в котором все цвета и картики, толщина и цвет бордеров)
       
       Если предполагается использование альтернативной таблицы стилей, имхо этот visuals.css очень удобен, потому что, прилинковывая alterscreen.css, который импортирует все тоже самое, кроме altervisuals.css можно сменить полностью визуальную презентацию, а если учесть, что я стараюсь не фиксировать в пикселях шрифты вообще (ну, когда это действительно нужно), то, еще раз, - очень удобно.
       
       [ просьба - если ты считаешь, на основе своего опыта, что я ошибаюсь - drop me a note, please :)]
       
       Эта штука работает и я думаю, что когда переключается скриптом на alterscreen.css в котором все файлы, кроме altervisuals.css теже самые - то они в кэше сидят уже :))
       
       Минусы
       приходится писать по нескольку раз один и тот же селектор в разных файлах, к примеру заголовок
       
       h2 {font-size:1.3em; font-family:Verdana, Arial, sans-serif;} в textformatting.css и
       
       h2 { color:#c60; background:#000 url(/);} в visuals.css
       
       что еще ничего, но по нескольку раз писать 
       body.clientprofile #content-primary #clientpassport #photoimg ( :) ) приводит у сайта размером с голубя :) к суммарному увеличению CSS файлов на 2 килобайта почти.
       
       Есть еще "минусы" связанные с тем, что кодеру придется как-то определяться (и лучше хорошо подумать, прикинув потребности сайта и пользователей, сразу) куда, например, относить тот же отступ заголовка к visuals или layout... It depends
       
       Но все равно, учитывая то, что файлы кэшируются, а так же грамотно применяя каскад и наследование наряду с селекторами типа *, размер CSS для "голубя" не вылазит за пределы 10-12 килобайт. Что, в свою очередь, оставляет за пределами профессионализма любой сайт, сверстанный методами "старой школы".

     email: "andrey.stefanenko@gmail.com"

  -  author: "akella"
     id: "2104"
     url: "http://cssing.iatp.org.ua"
     date: "2005-08-25 12:13:32"
     humandate: "25 Aug, 2005"
     content: | 
       Уххх, накатали ) Спасибо.
       2Ganges: ты затронул тему которой смело можно посвятить еще один пост. ) Собссно формат твоего комментария подходит)).
       Сказывается отсутствие блога...
       
       2 Агат: у тебя совсем минимал подход - я больший лентяй! :) Однозначно!

     email: "akella.a@gmail.com"

  -  author: "Van"
     id: "2114"
     url: "http://zoob.ru"
     date: "2005-08-29 12:06:42"
     humandate: "29 Aug, 2005"
     content: | 
       А вот это что должно обозначать?
       ...
       [meta http-equiv="Content-Type" content="text/html; charset=windows-1251" /]
       [meta http-equiv="Content-Type" content="text/html;charset=utf-8" /]
       ...

     email: "van@zoob.ru"

  -  author: "akella"
     id: "2115"
     url: "http://cssing.iatp.org.ua"
     date: "2005-08-29 12:19:45"
     humandate: "29 Aug, 2005"
     content: | 
       Я оставил в шаблоне 2 самые используемые кодировки - ненужную надо просто удалить - это проще чем дописать...

     email: "akella.a@gmail.com"

  -  author: "StraNNicK"
     id: "2125"
     url: "http://strannick.blogspot.com"
     date: "2005-08-31 10:42:47"
     humandate: "31 Aug, 2005"
     content: | 
       Привет. Не совсем в тему (вернее - совсем не в тему), но не могу не поделиться.
       Откопал совершенно шикарный (хотя и популистский) сайт.
       
       http://www.sitepoint.com/
       
       Правда чует моё сердце, что все про него давно знают, но вдруг... :)

     email: "strannick@gmail.com"

  -  author: "akella"
     id: "2126"
     url: "http://cssing.iatp.org.ua"
     date: "2005-08-31 11:13:40"
     humandate: "31 Aug, 2005"
     content: | 
       http://cssing.iatp.org.ua/resources/ ....
       ;)

     email: "akella.a@gmail.com"

  -  author: "polch"
     id: "2159"
     url: "http://www.tobto.com.ua/"
     date: "2005-09-01 10:48:38"
     humandate: "01 Sep, 2005"
     content: | 
       дробить css-файл на мелкие части - гуд, но лучше сделать файл миниатюрным. 
       А на sitepoint.com куча классных примеров. рекомендую настырно.

     email: "nebesna@bigmir.net"

  -  author: "akella"
     id: "2160"
     url: "http://cssing.iatp.org.ua"
     date: "2005-09-01 11:06:17"
     humandate: "01 Sep, 2005"
     content: | 
       Не всегда можно сделать миниатюрным... :(
       А что плохого в разделении? Так ведь удобней редактировать - год назад делал а схемы в голове...
       
       Минимизировать эт всегда надо...

     email: "akella.a@gmail.com"

  -  author: "memyself"
     id: "2268"
     url: "http://npj.ru/valine"
     date: "2005-09-07 16:56:04"
     humandate: "07 Sep, 2005"
     content: | 
       Насчёт дробления - главный недостаток в том, что увеличивается количество запросов к веб-серверу, а соответственно и нагрузка на сервер.

     email: "val.budkin@gmail.com"

  -  author: "akella"
     id: "2269"
     url: "http://cssing.iatp.org.ua"
     date: "2005-09-07 17:17:23"
     humandate: "07 Sep, 2005"
     content: | 
       Тут я рискну не согласиться: оно кешируется и этот фактор почти не играет роли - по крайней мере добавление 12 запросов(IMG) к главной странице укр.нет вообще никак не сказалось на производительности. А тут речь идет о 2х 3х...
       
       Так же как <strong>НЕ</strong>дробление, мне чуждо удаление пробелов и переводов строк в ЦСС... Себе в убыток - надо знать меру.

     email: "akella.a@gmail.com"

  -  author: "polch"
     id: "2290"
     url: "http://www.tobto.com.ua/"
     date: "2005-09-15 12:58:59"
     humandate: "15 Sep, 2005"
     content: | 
       решил и я сделать вклад в "братскую могилку" заготовок: 
       <ol class="code">
       <li>&lt;? echo="&lt;?xml version="1.0" encoding="iso-8859-1"?&gt;"; ?&gt;
       <li>&lt;!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
       <li>"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"&gt;</li>
       <li>&lt;html xmlns="http://www.w3.org/1999/xhtml"&gt;</li>
       <li>&lt;head&gt;</li>
       <li>&lt;title&gt;xxx&lt;/title&gt;</li>
       <li>&lt;meta http-equiv="Content-Type" content="text/html; charset=iso-8859-1" /&gt;</li>
       <li>&lt;style type="text/css"&gt;</li>
       <li>&lt;!--</li>
       <li>body {</li>
       <li class="tab"> font-family: Verdana, Arial, Helvetica, sans-serif;</li>
       <li class="tab"> font-size: 80%;</li>
       <li class="tab"> color: #333;</li>
       <li>}</li>
       <li>a {</li>
       <li class="tab"> color: #999;</li>
       <li class="tab"> text-decoration: none;</li>
       <li>}</li>
       <li>--&gt;</li>
       <li>&lt;/style&gt;</li>
       <li>&lt;/head&gt;</li>
       <li></li>
       <li>&lt;body&gt;</li>
       <li>&lt;/body&gt;</li>
       <li>&lt;/html&gt;</li>
       </ol>
       
       Должен сказать, что у меня их четыре - на случай разных кодировок и строгостей стандартов. 
       
       Относительно дробления, недавно вычитал у какого-то америкоза. Он дает минимальный стиль около 10 строчек, все, ессно, фиксд, но компилант со Всеми броузерами, включая раненый NN4! Красота. Минимум-миниморум. Но по идее надобы определять броузер и давать ему что он хочет. 
       
       Добавлю, что после дооолгих мучительных исследований cms, заприметил DataLife Engine российского производства. Впечатляет. Красиво, быстро, легко. Сейчас пытаюсь повыдергивать из него все таблицы и перевести дизайн на родной css. Addio.

     email: "nebesna@bigmir.net"

  -  author: "akella"
     id: "2350"
     url: "http://cssing.iatp.org.ua"
     date: "2005-09-26 17:10:42"
     humandate: "26 Sep, 2005"
     content: | 
       Речь не о структуре хтмл а скорее структуре ЦСС файлов - создавать каждый раз 5 или 6 штук - напряг - а так сразу и в папочке - так сказать выращиваю в себе культуру кодера...
       Вроде и мало что сделано в них - а психологически намного легче начать новый сайт делать.

     email: "akella.a@gmail.com"

  -  author: "Riff"
     id: "2349"
     url: "http://rifflog.com"
     date: "2005-09-26 00:57:54"
     humandate: "26 Sep, 2005"
     content: | 
       я конечно не спорю, что заготовки это хорошо... я и сам пытался их сделать... в итоге осталась тока одна с хэдером и доктайпом... почему? а потому что заготовки хороши только при наличии энного к-вы заказов с одинаковой блочной структурой, а в моём случае блоки н расположены как в голову шибанёт :)

     email: "riff@rifflog.com"

  -  author: "cssing :: Архив   :: CSS для непослушных броузеров"
     id: "2708"
     url: "http://cssing.org.ua/2006/01/17/hacks-in-separate-stylesheet/"
     date: "2006-01-17 15:29:06"
     humandate: "17 Jan, 2006"
     content: | 
       [...] файл. О том как я это делаю я и написал. Структура CSS файлов 	Если кто помнит(пост на эту тему), то я линкую из страниц на один CSS файл master.css. Примерно так [...]

     email: ""

  -  author: "Maxim"
     id: "10904"
     url: "http://www.rozhkov.com.ua"
     date: "2007-04-15 15:29:11"
     humandate: "15 Apr, 2007"
     content: | 
       битая ссылка http://cssing.iatp.org.ua/examples/template/template.rar :o(

     email: "maxim@rozhkov.com.ua"

  -  author: "Роман"
     id: "67795"
     url: ""
     date: "2012-07-06 23:20:15"
     humandate: "06 Jul, 2012"
     content: | 
       Для меня сейчас Заготовкой является запись html:5&gt;#wrap&gt;(#header+#middle+#footer)+"Tab"
       Zen-coding очень помогает верстать.
       Так же когда уж очень лень лезу сюда http://csstemplater.com/

     email: "1skatel@mail.ru"

  -  author: "Андрей"
     id: "31935"
     url: ""
     date: "2012-01-03 18:05:51"
     humandate: "03 Jan, 2012"
     content: | 
       html5 заготовка
       http://divhack.com/node/32

     email: "serj_life@list.ru"

layout: "layouts/post.njk"
excerpt: "На горизонте, как тучи, собирается работа... Решил не ждать - а начать готовиться. Подготовил серию XHTML заготовок."
---

На горизонте, как тучи, собирается работа... Решил не ждать - а начать готовиться. Подготовил серию XHTML заготовок.<!--more-->
<h3>Зачем?</h3>
Каждый раз когда я начинаю верстать, я заново ворую где то доктайп, создаю CSS файлы -  переписываю метатэги с какого-нить доверенного сайта. Но, наконец, чаша полна. Лень ослабла, и я решился сделать стартовые HTML+CSS заготовки. Кому сгодятся - используйте на здоровье...
<h3>HTML</h3>
Не буду тут приводить полностью файл. Однако я в него насовал все метатэги которые я использовал. Вот небольшой такой список:
<ol class="code">
<li>&lt;meta http-equiv="Content-Type" content="text/html; charset=windows-1251" /&gt;</li>

<li>&lt;meta http-equiv="Content-Language" content="ru" /&gt;</li>
<li>&lt;meta name="copyright" content="" /&gt;</li>
<li>&lt;meta name="description" content="" /&gt;</li>
<li>&lt;meta name="keywords" content="" /&gt;</li>
<li>&lt;meta name="author" content="" /&gt;</li>
<li>&lt;meta name="robots" content="all" /&gt;</li>
<li>&lt;link rel="Shortcut Icon" type="image/x-icon" href="/favicon.ico" /&gt;</li>
</ol>
Я выбирал самое нужное для себя - если у кого есть чем дополнить - пожалуйста в комменты...

Плюс ссылки на (смотри ниже) CSS файлы
<h3>CSS</h3>
Главная страница ссылается на 3 CSS файла: <strong>master.css print.css handheld.css</strong>. Которые все лежат в папке <strong>css</strong>.

Содержание master.css примерно такое:
<ol class="code">
<li>@import url("base.css");</li>
<li>@import url("layout.css");</li>
</ol>
И еще сколько влезет разделений на стили для <strong>цвета</strong>, <strong>шрифтов</strong>.
Просто я использую пока именно такое разделение.

Все CSS файлы снабжены заботливо спертыми заголовками у Дага Баумана (нравятся они мне :)) Вот такого вида:
<ol class="code">
<li>/*</li>
<li>-----------------------------------------------</li>
<li>Site Screen Master</li>
<li>Author:   akella</li>
<li>Version:  28 Apr 1983</li>
<li>----------------------------------------------- */</li>
</ol>

<h3>Результат</h3>
В результате вышло такое:
<img alt="file tree of template" src="http://cssing.org.ua/images/tree.png"  style="border:none;" />
Скачать все сразу можно <a href="http://cssing.org.ua/examples/template/template.rar">отсюда</a>. Посмотреть вживую - <a href="http://cssing.org.ua/examples/template/">тут</a>. (нажимайте вью сорс)
Для маленьких сайтов(воробьев) - это конечно скорее пушка, но для средних проектов самое то. Да и пушкой в принципе убить воробья - не так и трудно :).
<h3>Инфо</h3>
<ul>
<li><a href="http://www.digital-web.com/articles/architecting_css/">Architecting CSS</a></li>
<li><a href="http://particletree.com/features/quick-start-your-design-with-xhtml-templates">XHTML templates</a></li>
</ul>

Замечания-указания-поправки с радостью принимаются )
