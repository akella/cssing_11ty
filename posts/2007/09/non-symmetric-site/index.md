---
title: "Несимметричный фон на центрированном сайте"
date: "2007-09-29"
humanDate: "29 Sep, 2007"
permalink: "2007/09/29/non-symmetric-site/"
tags: 
  - "xhtmlcss"
comments: 
  -  author: "pepeplsbey"
     id: "11172"
     url: "http://pepelsbey.net/"
     date: "2007-09-30 08:44:45"
     humandate: "30 Sep, 2007"
     content: | 
       Если картинка довольно простая, то можно просто создать её из требуетмых половинок очень (ну очень) большой в ширину, сохранить в PNG-8 и положить со смещением 50% на BODY.
       
       Пару раз так делал, вполне себе удобно.

     email: "pepelsbey@gmail.com"

  -  author: "Mourner"
     id: "11173"
     url: "http://agafonkin.com"
     date: "2007-09-30 11:47:03"
     humandate: "30 Sep, 2007"
     content: | 
       Блин, не додумался в своё время, спасибо за совет!
       
       Делал всегда как указал pepelsbey, но в этом решении нельзя поспользоваться преимуществом repeat-x, а картинка большая всё-таки больше весит одного пикселя.

     email: "agafonkin@gmail.com"

  -  author: "akella"
     id: "11174"
     url: "http://cssing.org.ua"
     date: "2007-09-30 15:11:29"
     humandate: "30 Sep, 2007"
     content: | 
       Да - полностью согласен насчет большой(широкой) картинки. Хотя пересев за 20" Аймак я слегка разочаровался в этой идее на некоторых сайтах :) Большое разрешение балует...

     email: "akella.a@gmail.com"

  -  author: "Сергей"
     id: "11175"
     url: "http://strategiya-biznesa.info"
     date: "2007-09-30 21:06:36"
     humandate: "30 Sep, 2007"
     content: | 
       Спасибо. Хороший совет. Как и все остальные :)

     email: "admi@strategiya-biznesa.info"

  -  author: "Local"
     id: "11176"
     url: "http://dlocal.livejournal.com"
     date: "2007-10-01 05:06:48"
     humandate: "01 Oct, 2007"
     content: | 
       Полезная статья, пригодится, спасибо.

     email: "den.local@gmail.com"

  -  author: "akira"
     id: "11177"
     url: "http://akira.spb.su"
     date: "2007-10-01 09:58:34"
     humandate: "01 Oct, 2007"
     content: | 
       Мне кажется или ссылка одинаковые? :-)

     email: "akira@phpcom.ru"

  -  author: "akella"
     id: "11178"
     url: "http://cssing.org.ua"
     date: "2007-10-01 10:56:08"
     humandate: "01 Oct, 2007"
     content: | 
       в index1.html у меня серые блоки поверх текста... а в каком броузере обе ссылки одинаково выглядят?

     email: "akella.a@gmail.com"

  -  author: "Ivan"
     id: "11179"
     url: ""
     date: "2007-10-02 09:21:03"
     humandate: "02 Oct, 2007"
     content: | 
       Akella, это все хорошо. Но мне интересно, как бы ты реализовал точно такую же ситуацию, но с учетом того, что фон разный и справа и слева должен тянуться на 100% по высоте.
       
       Вечером отпишу свое решение, сейчас под рукой нету исходников.

     email: "itouring@gmail.com"

  -  author: "akella"
     id: "11180"
     url: "http://cssing.org.ua"
     date: "2007-10-02 14:33:32"
     humandate: "02 Oct, 2007"
     content: | 
       Первое что приходит в голову
       body{padding-left:20%}
       #out{padding-right:20%}
       Ну и соответственно фоны задавать для БОДИ и #out. Их протяженность по вертикали уже можно контролировать

     email: "akella.a@gmail.com"

  -  author: "Cooluck"
     id: "11181"
     url: "http://6104.org.ua"
     date: "2007-10-03 11:57:01"
     humandate: "03 Oct, 2007"
     content: | 
       <a href="http://fotki.yandex.ru/users/cooluck/view/12363" rel="nofollow"></a><a href="http://fotki.yandex.ru/users/cooluck/view/12363" rel="nofollow">«Глюк?»</a> на <a href="http://fotki.yandex.ru" rel="nofollow">Яндекс.Фотках</a>
       
       И ссылки у меня тоже одинаковые, кликал из Feedreader

     email: "wheelcity@ya.ru"

  -  author: "akella"
     id: "11183"
     url: "http://cssing.org.ua"
     date: "2007-10-04 17:47:11"
     humandate: "04 Oct, 2007"
     content: | 
       Хм - а в моих виндошных все ок... что у тебя за броузер?

     email: "akella.a@gmail.com"

  -  author: "Cooluck"
     id: "11184"
     url: "http://blog.cooluck.kiev.ua/"
     date: "2007-10-04 22:26:45"
     humandate: "04 Oct, 2007"
     content: | 
       ИЕ 6, стандартная сборка.

     email: "wheelcity@ya.ru"

  -  author: "akella"
     id: "11185"
     url: "http://cssing.org.ua"
     date: "2007-10-05 10:32:03"
     humandate: "05 Oct, 2007"
     content: | 
       Странно - на моей чистой WinXP - все ок в ИЕ6 (

     email: "akella.a@gmail.com"

  -  author: "Tween"
     id: "11186"
     url: "http://yandex.ru/"
     date: "2007-10-05 12:37:24"
     humandate: "05 Oct, 2007"
     content: | 
       В общем-то то же самое можно и таблицами сверстать. Или CSS-Таблицами ,если уж все так любят DIV:)

     email: "ttion@mail.ru"

  -  author: "akella"
     id: "11187"
     url: "http://cssing.org.ua"
     date: "2007-10-05 12:54:08"
     humandate: "05 Oct, 2007"
     content: | 
       На этом блоге нет обсуждений как верстать - таблицами или нет =). И я никого не буду уговаривать...

     email: "akella.a@gmail.com"

  -  author: "Tween"
     id: "11189"
     url: "http://yandex.ru/"
     date: "2007-10-05 23:07:19"
     humandate: "05 Oct, 2007"
     content: | 
       В смысле имелось ввиду ,решить проблему наверняка можно ещё проще=)

     email: "ttion@mail.ru"

  -  author: "akella"
     id: "11190"
     url: "http://cssing.org.ua"
     date: "2007-10-05 23:20:19"
     humandate: "05 Oct, 2007"
     content: | 
       При всем уважении - вряд ли. Решение при помощи кучи лишнего кода для меня не более простое решение. Даже добавление пустого дива ) нож по сердцу. Я уж молчу о таблице с тремя ячейками, в которой я запутаюсь очень быстро =)

     email: "akella.a@gmail.com"

  -  author: "Cooluck"
     id: "11192"
     url: "http://cooluck.kiev.ua"
     date: "2007-10-06 00:52:55"
     humandate: "06 Oct, 2007"
     content: | 
       Проявляется данный глюк на самом крупном размере шрифта, как оказалось.
       По-моему из-за слова Несимметричный его "распирает"

     email: "wheelcity@ya.ru"

  -  author: "karasik"
     id: "11241"
     url: ""
     date: "2007-10-26 16:33:50"
     humandate: "26 Oct, 2007"
     content: | 
       Ivan сказал(а) 2 октября:
       
        Akella, это все хорошо. Но мне интересно, как бы ты реализовал точно такую же ситуацию, но с учетом того, что фон разный и справа и слева должен тянуться на 100% по высоте.
       
        Вечером отпишу свое решение, сейчас под рукой нету исходников.
       
       Так как же все-таки это сделать? Очень нужно .. пока что не нашел решения
       
       За инфу - большое СПС

     email: "y-evt@yandex.ru"

  -  author: "akella"
     id: "11242"
     url: "http://cssing.org.ua"
     date: "2007-10-26 21:33:36"
     humandate: "26 Oct, 2007"
     content: | 
       Так в 9м каменте я вроде бы постарался описать свое решение.
       Иван?

     email: "akella.a@gmail.com"

  -  author: "karasik"
     id: "11245"
     url: ""
     date: "2007-10-29 12:13:22"
     humandate: "29 Oct, 2007"
     content: | 
       2akella:
       что касается "9" - все ясно.
       
       Надеялся на решение которое позволит использовать левый и правый дивы в качестве "ушек", т.к. бэкграунд на боди уже занят ))
       
       и еще вопросик(сорри за оффтоп):
       можно ли сделать так чтобы заканчивался не под , а возле его края ... при условии что ширина фиксированная?

     email: "y-evt@yandex.ru"

  -  author: "akella"
     id: "11247"
     url: "http://cssing.org.ua"
     date: "2007-10-29 14:31:49"
     humandate: "29 Oct, 2007"
     content: | 
       Напиши мне на имейл внизу страницы, а то я не очень понимаю что ты хочешь сделать...

     email: "akella.a@gmail.com"

  -  author: "karasik"
     id: "11273"
     url: ""
     date: "2007-11-06 16:26:22"
     humandate: "06 Nov, 2007"
     content: | 
       2akella
       Спасибо, проблема была решена другими методами.

     email: "y-evt@yandex.ru"

  -  author: "Del'ka"
     id: "12418"
     url: ""
     date: "2008-05-15 13:25:35"
     humandate: "15 May, 2008"
     content: | 
       в IE не работает(

     email: "delka@anime.kharkov.ua"

  -  author: "Del'ka"
     id: "12419"
     url: ""
     date: "2008-05-15 13:27:19"
     humandate: "15 May, 2008"
     content: | 
       ага, увидел в самом низу пример где для IE используется filter - красиво!
       взял на вооружение)

     email: "delka@anime.kharkov.ua"

  -  author: "aga"
     id: "14261"
     url: ""
     date: "2009-03-11 15:31:08"
     humandate: "11 Mar, 2009"
     content: | 
       Засунули весь сайт в один див и радуются, обсуждают как круто получилось! Я бы за такое как минимум пропесочил верстальщика, как максимум выгнал с работы.

     email: "aga@ugu.da"

  -  author: "Несимметричный фон на центрированном сайте &laquo; Articles about Web Development"
     id: "12930"
     url: "http://tobecomeprofy.wordpress.com/2007/10/01/%d0%bd%d0%b5%d1%81%d0%b8%d0%bc%d0%bc%d0%b5%d1%82%d1%80%d0%b8%d1%87%d0%bd%d1%8b%d0%b9-%d1%84%d0%be%d0%bd-%d0%bd%d0%b0-%d1%86%d0%b5%d0%bd%d1%82%d1%80%d0%b8%"
     date: "2008-07-18 23:51:15"
     humandate: "18 Jul, 2008"
     content: | 
       [...] Читаем [...]

     email: ""

layout: "layouts/post.njk"
excerpt: "Относительно часто встречаются макеты центрированные по горизонтали, но с уходящими влево и вправо разнымы фоновыми картинками, <a href=\"http://cssing.org.ua/examples/unsymbg/\">примерно так</a>.

Делюсь своим способом решения этой задачи.
"
---

Относительно часто встречаются макеты центрированные по горизонтали, но с уходящими влево и вправо разнымы фоновыми картинками, <a href="http://cssing.org.ua/examples/unsymbg/">примерно так</a>.

Делюсь своим способом решения этой задачи.
<!--more-->
<h3>Конечный результат</h3>
Добиваться будем примерно <a href="/examples/unsymbg/">следующего</a>.

Кто понимает код - можно дальше и не читать =)
<h3>Центрирование</h3>
Вообще классическое центрирование обычно выглядит так:
<strong>HTML:</strong>
<ol class="code">
<li>&lt;body&gt;</li>
<li class="tab">&lt;div id=&quot;out&quot;&gt;</li>
<li class="tabtab">...сайт...</li>
<li class="tab">&lt;/div&gt;</li>
<li>&lt;/body&gt;</li>
</ol>
<strong>CSS:</strong>
<ol class="code">
<li>body{text-align:center}</li>
<li>#out{</li>
<li class="tab">width:700px;</li>
<li class="tab">margin: 0 auto;</li>
<li>}</li>
</ol>
Почему-то все еще часто можно услышать вопросы о центрировании или применении тага <code>CENTER</code>, потому не лишне наверно было упомянуть эту реализацию =)
<h3>несимметричный фон</h3>
Для реализации придется добавить пустой див(это стыдно и неправильно, да):
<ol class="code">
<li>&lt;body&gt;</li>
<li><strong>&lt;div class=&quot;stupid-right&quot;&gt;&lt;/div&gt;</strong></li>
<li class="tab">&lt;div id=&quot;out&quot;&gt;</li>
<li class="tabtab">...сайт...</li>
<li class="tab">...</li>
</ol>
и соответствующий этому диву CSS:
<ol class="code">
<li>.stupid-right{</li>
<li class="tab">position:absolute</li>
<li class="tab">top:0;</li>
<li class="tab">right:0;<small>/*правый верхний угол */</small></li>
<li class="tab">width:50%;<small>/*половина экрана */</small></li>
<li class="tab">height:200px;</li>
<li class="tab">background:green;</li>
<li>}</li>
</ol>
Таким образом див берется шириной в половину экрана, и позиционируется в правый верхинй угол, а значит никогда не будет вылазить слева от сайта, ни при каких разрешениях.
Добавив такой же блок слева, получим вот что-то <a href="/examples/unsymbg/index1.html">вроде этого (дивы перекроют по половине сайта справа и слева)</a>:

Добавим:
<ol class="code">
<li>#out{</li>
<li class="tab">position:relative;</li>
<li>}</li>
</ol>
Таким образом мы поменяли их местами "в третьем" измерении, и все <a href="/examples/unsymbg/">выглядит как надо</a>.

<h3>В конце</h3>
Паттерн до боли простой, если кто-то решал подобную задачу по другому, был бы рад опыту.
<ul>
<li><a  href="/examples/unsymbg/">Пример с разными фонами с обеих сторон</a></li>
</ul>
