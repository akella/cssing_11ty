---
title: "Какие-то сложные игры c флоатами"
date: "2008-08-29"
humanDate: "29 Aug, 2008"
permalink: "2008/08/29/float-mess/"
tags: 
  - "xhtmlcss"
comments: 
  -  author: "YoYurec"
     id: "13157"
     url: "http://yoyurec.in.ua"
     date: "2008-08-29 11:27:30"
     humandate: "29 Aug, 2008"
     content: | 
       ну вы, ребята, и маньяки!!!
       одним словом - изящно.
       
       &gt;Всегда полезно общаться с иностранными коллегами.
       приятно также, что доносят знания и дополняют их наши коллеги :)
       
       ещё раз спсб!

     email: "yoyurec@gmail.com"

  -  author: "vladfrandom"
     id: "13155"
     url: ""
     date: "2008-08-29 10:51:08"
     humandate: "29 Aug, 2008"
     content: | 
       вместо всей этой красоты для IE хватило бы:
       
       /*Стили только для IE*/
       dt,dd{clear:right;}

     email: "randf@mail.ru"

  -  author: "akella"
     id: "13156"
     url: "http://cssing.org.ua"
     date: "2008-08-29 10:54:55"
     humandate: "29 Aug, 2008"
     content: | 
       Круто! Спасибо! И правда работает, не знаешь <em>почему</em>? =)
       Или уже сталкивался с такой задачей и опытным путем..?

     email: "akella.a@gmail.com"

  -  author: "vladfrandom"
     id: "13160"
     url: ""
     date: "2008-08-29 20:30:57"
     humandate: "29 Aug, 2008"
     content: | 
       опыт... пригодилость для карусельного слайдшоу.
       а вот почему... it's IE, be ready, here begins the strange miracles
       кстати Тьерри дал невалидный вариант.

     email: "randf@mail.ru"

  -  author: "akella"
     id: "13161"
     url: "http://cssing.org.ua"
     date: "2008-08-29 20:41:33"
     humandate: "29 Aug, 2008"
     content: | 
       Кое-как мне удалось найти в этом логику "уж если ты clear:right; то не смей сползать под float:left!"
       Я так и написал "грязный", я не фанат ЦСС-валидности, я практик работавший в стрессовых ситуациях =) Просто одна из альтернатив для _ и $

     email: "akella.a@gmail.com"

  -  author: "Vii"
     id: "13162"
     url: ""
     date: "2008-08-29 23:40:55"
     humandate: "29 Aug, 2008"
     content: | 
       Немножко не в тему, но для IE ведь еще можно писать: *float:none; (если я не ошибаюсь, это "чудо" понимают и 6-ой, и 7-ой)

     email: "d1gital_nek@land.ru"

  -  author: "vladfrandom"
     id: "13163"
     url: ""
     date: "2008-08-29 23:44:06"
     humandate: "29 Aug, 2008"
     content: | 
       скорее такое поведение имеет общие корни с эффектом height:1%; для родителя флоаченых элементов или vertcal-align:top; для вертикального списка с блочніми линками. imho естественно

     email: "randf@mail.ru"

  -  author: "vladfrandom"
     id: "13165"
     url: ""
     date: "2008-08-29 23:50:36"
     humandate: "29 Aug, 2008"
     content: | 
       и, да, я маньяк валидности кода. хотя и работаю на верстальном конвейере =)

     email: "randf@mail.ru"

  -  author: "Олег"
     id: "13170"
     url: "http://www.htmlverstka.ru"
     date: "2008-08-30 23:27:11"
     humandate: "30 Aug, 2008"
     content: | 
       &gt; "dt,dd,{float:none;}/*лишняя запятая*/"
       а смысл хака, есть универсальный, можно просто добавить знак $ и это поймут только ИЕ, например: $dt,$dd {float:none;}

     email: "a11_1@mail.ru"

  -  author: "akella"
     id: "13171"
     url: "http://cssing.org.ua"
     date: "2008-08-30 23:40:06"
     humandate: "30 Aug, 2008"
     content: | 
       Олег, то что вы написали не работает. Это не поймет ни один броузер.
       Правильно dt,dd{$float:none}.

     email: "akella.a@gmail.com"

  -  author: "Deff"
     id: "13172"
     url: "http://htmlcsscoder.com"
     date: "2008-08-31 00:09:11"
     humandate: "31 Aug, 2008"
     content: | 
       Или я что-то пропустил, или пример Тиерри в опере 9.5 таки сползает. И не при минимальном размере окна. А вот пример Влада более стабилен

     email: "info@htmlcsscoder.com"

  -  author: "xain"
     id: "13177"
     url: "http://www.brusmast.com.ua"
     date: "2008-08-31 18:00:16"
     humandate: "31 Aug, 2008"
     content: | 
       Юрий, а почему ты не выкладываеш свои кросс-посты на www.habrahabr.ru - я думаю людям будет очень приятно почитать твои статьи, сам читаю с удовольствием.

     email: "xain@yandex.ua"

  -  author: "akella"
     id: "13178"
     url: "http://cssing.org.ua"
     date: "2008-08-31 21:12:33"
     humandate: "31 Aug, 2008"
     content: | 
       Мне не нравится идея дублирования контента, а выкладывать там только ссылку сюда это какой-то чуждый мне пиар.

     email: "akella.a@gmail.com"

  -  author: "Евгений"
     id: "13187"
     url: ""
     date: "2008-09-01 17:46:25"
     humandate: "01 Sep, 2008"
     content: | 
       Отличный пример — спасибо!
       
       Впрочем как всегда… =)

     email: "yaumail@bk.ru"

  -  author: "Nit"
     id: "13201"
     url: "http://spamparampampam.com/"
     date: "2008-09-03 20:22:56"
     humandate: "03 Sep, 2008"
     content: | 
       Мне понравилось, классный пример, я уже и применить как придумал

     email: "bld@mail.ru"

  -  author: "0Т0"
     id: "13202"
     url: "http://oto-studio.com"
     date: "2008-09-03 22:26:24"
     humandate: "03 Sep, 2008"
     content: | 
       Юра, простите, что не по теме. 
       Хочу узнать ваше мнение относительно данной верстки: http://oto-studio.com/lenta/
       Любопытно.
       Спасибо.

     email: "den@oto-studio.com"

  -  author: "Genn"
     id: "13206"
     url: "http://genn.org/"
     date: "2008-09-04 08:43:28"
     humandate: "04 Sep, 2008"
     content: | 
       Очень интересный пост. Автор показался раскрыть со всех сторон тему. Мне кажется, что ему это удалось. Раньше зависал на других сайтах, но узнал об этом.

     email: "soap@genn.org"

  -  author: "Genn"
     id: "13207"
     url: "http://genn.org/"
     date: "2008-09-04 08:48:14"
     humandate: "04 Sep, 2008"
     content: | 
       Кстати, проверь в Гуглохроме на всякий случай. Мне кажется, что эта компания энтузиастов придумала-таки, как подложить всем свиней ;)

     email: "soap@genn.org"

  -  author: "akella"
     id: "13208"
     url: "http://cssing.org.ua"
     date: "2008-09-04 14:47:48"
     humandate: "04 Sep, 2008"
     content: | 
       @OTO: табличная верстка. Для пользователя, почти никакой разницы, кроме слегка дерганой загрузки, как всегда с таблицами. 
       С технической точки зрения &#8212; много необязательных таблиц, как следствие неоправданные усложнения читабельности и сложности кода.
       Так же обязательно нужно начать использовать таг P.
       В остальном все клево.
       
       @Genn: да нет, таки нет, по крайней мере в этом случае, обычный webkit. Просто не последняя версия.

     email: "akella.a@gmail.com"

  -  author: "hitalex"
     id: "13209"
     url: "http://spamparampampam.com/"
     date: "2008-09-05 01:03:31"
     humandate: "05 Sep, 2008"
     content: | 
       Думаю все-таки придумано очень даже интересно. Правда с другой стороны это искусство ради искусства.

     email: "hitalex0@gmail.com"

  -  author: "0Т0"
     id: "13214"
     url: "http://oto-studio.com"
     date: "2008-09-05 22:26:10"
     humandate: "05 Sep, 2008"
     content: | 
       Благодарю.

     email: "den@oto-studio.com"

  -  author: "cross"
     id: "13225"
     url: "http://blog.itcross.net/"
     date: "2008-09-09 18:18:16"
     humandate: "09 Sep, 2008"
     content: | 
       Ох ничего себе :) Подобных манимуляций с dd тегами еще не видел )

     email: "itwebcross@gmail.com"

  -  author: "Дизель генератор"
     id: "13235"
     url: "http://spamparampampam.com/"
     date: "2008-09-15 11:49:16"
     humandate: "15 Sep, 2008"
     content: | 
       Интересная игра с тэгами...
       
       СПАСИБО!

     email: "pues@mail.ru"

  -  author: "Kelly"
     id: "13239"
     url: "http://spamparampampam.com/"
     date: "2008-09-16 21:25:44"
     humandate: "16 Sep, 2008"
     content: | 
       А по-моему, ничего особенного от ресайзинга и не произошло. Зря автор так сильно кричал Oh my god!

     email: "kel1984@gmail.com"

  -  author: "Роман"
     id: "13345"
     url: "http://menzone.ru"
     date: "2008-10-02 14:06:28"
     humandate: "02 Oct, 2008"
     content: | 
       Интересно вот что: в вашем примере каждый блок является отдельным Definition list. Что не логично и "несемантично". А логично было бы, мне кажется, заключить ВСЕ элементы в один DL. Правда в таком случае вам уже не удастся не использовать обтекание (float) для DT и DD.

     email: "granturismo@mail.ru"

  -  author: "akella"
     id: "13346"
     url: "http://cssing.org.ua"
     date: "2008-10-02 14:09:05"
     humandate: "02 Oct, 2008"
     content: | 
       @Роман: в спецификации вообще говорится что DT должен быть один внутри DL ;)

     email: "akella.a@gmail.com"

  -  author: "Роман"
     id: "13350"
     url: "http://menzone.ru"
     date: "2008-10-03 21:57:59"
     humandate: "03 Oct, 2008"
     content: | 
       Вы не могли укать где именно так говорится? http://www.w3.org/TR/html401/struct/lists.html#h-10.3

     email: "granturismo@mail.ru"

  -  author: "akella"
     id: "13353"
     url: "http://cssing.org.ua"
     date: "2008-10-04 00:37:17"
     humandate: "04 Oct, 2008"
     content: | 
       Да, это я что-то сам придумал, прошу прощения =) Кажется где-то в WSG проскакивало, а контекст забыл. Наверное неверно отложилось. =(
       В любом случае мне кажется логичным оборачивать так =) да и удобнее стилизовать, вы правы.
       
       ЗЫ: кстати метод вполне сошел бы, только не удалось бы контролировать, чтобы дата и текст к ней относящийся был на одной строке =(

     email: "akella.a@gmail.com"

  -  author: "Андрей"
     id: "13547"
     url: "http://www.woolfs.ru"
     date: "2008-11-13 16:40:19"
     humandate: "13 Nov, 2008"
     content: | 
       Отличный пост, много новичков спрашивают именно подобные вопросы про слои. Помню как сам искал ответы на вёрстку и похожие темы нигде особо не были раскрыты.
       Ставлю ссылку на пост :)

     email: "woolfs@bk.ru"

  -  author: "cssing :: Архив :: CSSing 2008"
     id: "13896"
     url: "http://cssing.org.ua/2008/12/30/cssing-2008/"
     date: "2008-12-30 17:46:18"
     humandate: "30 Dec, 2008"
     content: | 
       [...] ? акие-то сложные игры c флоатами &#8212; по-другому и правда не скажешь. Необычный clear&#8217;инг [...]

     email: ""

layout: "layouts/post.njk"
excerpt: "По-другому и правда не назовешь. Ах, эта обманчивая внешняя простота:
<p class=\"img con\"><img src=\"http://cssing.org.ua/pic/floatmess/1.png\" alt=\"конечный результат\" /><span>Всё красиво</span></p>"
---

По-другому и правда не назовешь. Ах, эта обманчивая внешняя простота:
<p class="img con"><img src="http://cssing.org.ua/pic/floatmess/1.png" alt="конечный результат" /><span>Всё красиво</span></p><!--more-->
<h3>Всё просто</h3>
Скриншот нашей цели видно выше. Казалось бы, очевидным кодом будет:
<ol class="code">
<li>&lt;dl&gt;</li>
<li class="tab">&lt;dt&gt;42&lt;/dt&gt;</li>
<li class="tab">&lt;dd&gt;</li>
<li class="tabtab">&lt;strong&gt;Ответ на Вопрос&lt;/strong&gt;</li>
<li class="tabtab">&lt;a href=&quot;#&quot;&gt;Купить&lt;/a&gt;</li>
<li class="tab">&lt;/dd&gt;</li>
<li>&lt;/dl&gt;</li>
</ol>
Добавим такой CSS:
<ol class="code">
<li>dl,dt,dd{</li>
<li class="tab">float:left;<small>/*флоатим каждый из блоков DL, и оба подблока DT DD*/</small></li>
<li class="tab">}</li>
<li>dd strong{</li>
<li class="tab">display:block;<small>/*чтобы название товара и кнопка &laquo;купить&raquo; были на разных строках*/</small></li>
<li class="tab">}</li>
</ol>
Добавив еще <a href="http://cssing.org.ua/examples/floatmess/beauty.css">шрифтов и цветов</a> получим это:
<p class="img con"><img src="http://cssing.org.ua/pic/floatmess/1.png" alt="конечный результат" /><span>Ничто не предвещало беды</span></p>
<h3>Oh my... not again =(</h3>
Однако, вот что происходит при ресайзе окна:
<p class="img con"><img src="http://cssing.org.ua/pic/floatmess/2.png" alt="так выглядит в ИЕ" /><span>Так выглядит в ИЕ</span></p>
Как видите, блоки в панике, и не могут найти себе места. Не хватает только знаменитого крика &laquo;А-а-а-а-а&raquo;.
Признаюсь, после получаса тщетных усилий чувство паники овладело и мной. Я решил обратиться к умным ребятам в WSG.
<h3>WSG to the rescue!</h3>
Одно из замечательнейших онлайн сообществ на этой планетке. Веселые австралийцы там спорят о том &laquo;как делать сайты для слепых&raquo;, &laquo;каким HTML лучше размечать логотип&raquo;, и &laquo;что такое эти веб-стандарты в честь которых назвали наше сообщество&raquo;. Но там всегда помогают умным CSS-советом.

Калифорнийский француз, многодетный отец (2!) и вообще положительный человек <a href="http://www.tjkdesign.com/">Thierry</a>, как настоящий воин, не смог пройти мимо моей трудной задачи, и придумал своё решение. Все оказалось до постыдного простым, блоки нужно сделать inline, и задать white-space:nowrap;
Вот такой код нужно было добавить к первоначальному, чтобы все заработало:
<ol class="code">
<li>/*Стили только для IE*/</li>
<li>dt,dd{float:none;} <small>/*убираем флоаты*/</small></li>
<li>dt,dd{display:inline;zoom:1;} <small>/*делаем DT и DD инлайновыми, но zoom наделяет их возможностью padding и другими блочными свойствами*/</small></li>
<li>dl{white-space:nowrap;}<small>/*заставляем DT и DD быть на одной строке*/</small></li>
</ol>
Попутно, Тьерри поделился забавным ИЕ хаком (из разряда грязных):
<ol class="code"><li>dt,dd,{float:none;}<small>/*лишняя запятая*/</small></li></ol>
Вся строка будет понята только IE6-7.
Всегда полезно общаться с иностранными коллегами.
Спасибо <a href="http://www.tjkdesign.com/">Thierry</a>! <a href="http://cssing.org.ua/examples/floatmess/floatdl_thierry.html">Вот подправленный и теперь уже рабочий пример</a>.

Идея и код очень простые, но именно потому могут кому-то пригодиться.
<h3>Еще об этом</h3>
Изначально я пытался решить проблему CSS-таблицами, но к сожалению мне не удавалось сэмулировать это поведение для ИЕ:
<ol class="code">
<li>dl{display:table} </li>
<li>dt, dd{display:table-cell}</li>
</ol>
Это чтобы они вообще ни при каких обстоятельствах не переносились. При сильном сжатии окна, во всех предыдущих примерах, DD таки соскакивал вниз. При таком CSS, не соскакивает. <a href="http://cssing.org.ua/examples/floatmess/floatdl_akella.html">Пример</a>.
<h3>И еще вариант!</h3>
Как круто и гениально посоветовал в комментариях Влад, все это можно было бы решить вообще одной строкой для ИЕ:
<ol class="code">
<li>dt,dd{clear:right}</li>
</ol>
Совершенно непонятно почему, что, впрочем, не редкость с ИЕ, но <a href="http://cssing.org.ua/examples/floatmess/floatdl_vlad.html">это работает</a>&nbsp;=).
Великолепно иметь в запасе сразу две простых идеи решения такой задачи.
<h3>В конце</h3>
Хотя проблема специфична, она связана с &laquo;флоатами в одну строку&raquo;.  Что, вобщем, встречается нередко. Никогда не знаешь где может пригодиться inline или clear.
Интересной проблема мне показалась еще и  из-за внешней простоты дизайна.
<ul>
<li><a href="http://cssing.org.ua/examples/floatmess/normal.html">Первый глючный пример</a></li>
<li><a href="http://cssing.org.ua/examples/floatmess/floatdl_thierry.html">Пример от Тьерри</a> с display:inline</li>
<li><a href="http://cssing.org.ua/examples/floatmess/floatdl_akella.html">Третий пример</a> с table-cell</li>
<li><a href="http://cssing.org.ua/examples/floatmess/floatdl_vlad.html">Пример от vladfrandom</a> c clear:right</li>
</ul>
Буду рад если поделитесь своими мыслями по теме! Или задачами =)
