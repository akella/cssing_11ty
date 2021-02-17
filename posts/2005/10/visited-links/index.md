---
title: "Посещенные ссылки"
date: "2005-10-26"
humanDate: "26 Oct, 2005"
permalink: "2005/10/26/visited-links/"
tags: 
  - "xhtmlcss"
  - "design"
comments: 
  -  author: "Flightsnormal"
     id: "2470"
     url: "http://www.livejournal.com/users/flightsnormal/"
     date: "2005-10-27 04:49:39"
     humandate: "27 Oct, 2005"
     content: | 
       то же можно сделать видным и в ie
       просто использовать 
       
       background: url("galka.gif") no-repeat right; 
       padding-right: 1em;
       
       Возникает другой вопрос - как юзеру понять что ссылки с галками - это посещенные ссылки?

     email: "fnormal@gmail.com"

  -  author: "kost"
     id: "2471"
     url: "http://reg.kost.ru"
     date: "2005-10-27 09:12:12"
     humandate: "27 Oct, 2005"
     content: | 
       Поймут юзеры.
       
       А если не поймут, то и дефолтные фиолетовые ссылки им не помогут.

     email: "kost@kost.ru"

  -  author: "akella"
     id: "2472"
     url: "http://cssing.iatp.org.ua/"
     date: "2005-10-27 16:20:00"
     humandate: "27 Oct, 2005"
     content: | 
       Мне честно говоря больше нравится именно то что эта галочка сделана честным шрифтом - и где она ни появись на странице, подстроится под окружающий шрифт.
       
       А насчет понимания - никто ж не говорил что посещенные будем выделять только галочкой - цвет и подчеркивания к нашим услугам...

     email: "akella.a@gmail.com"

  -  author: "Sly"
     id: "2477"
     url: ""
     date: "2005-10-28 21:15:12"
     humandate: "28 Oct, 2005"
     content: | 
       Какая разница между a:visited и a:visited:after?

     email: "sly@ag.ru"

  -  author: "ganges"
     id: "2482"
     url: ""
     date: "2005-10-31 12:21:08"
     humandate: "31 Oct, 2005"
     content: | 
       В 
       :after 
       ты сможешь "сгенерировать" нужное тебе содержимое после ссылки. в то время как в просто :visited - ты можешь работать только непосредственно с самой (посещенной) ссылкой
       
       Псевдокласс :after не поддерживается даже в ИЕ 6.0

     email: "andrey.stefanenko@gmail.com"

  -  author: "Никита"
     id: "2527"
     url: "http://www.umade.ru/"
     date: "2005-11-03 19:11:23"
     humandate: "03 Nov, 2005"
     content: | 
       Интересно получается :)
       
       <a href="http://www.umade.ru/log/2005/09/110.html" rel="nofollow">Посещенные ссылки. Visited links</a>

     email: "hello@umade.ru"

  -  author: "akella"
     id: "2540"
     url: "http://cssing.iatp.org.ua/"
     date: "2005-11-05 12:08:27"
     humandate: "05 Nov, 2005"
     content: | 
       Пардон, коллега, - так увлекся зарубежными блогами, что про своих стал забывать.... (. Извини - за всеми не уследил... :(

     email: "akella.a@gmail.com"

  -  author: "Vadim"
     id: "3326"
     url: ""
     date: "2006-05-24 18:59:55"
     humandate: "24 May, 2006"
     content: | 
       Пост оставлен 26 октября, 2005 года в 5:42 pm в категории XHTML/CSS, Дизайн - akella сказал(а):
       
       quote-----
       Вот такие красивые радикальчики-галочки. Среди символов есть и настоящая “галочка” (check mark) - ***он она***, к сожалению, отображается далеко не во всех броузерах..
       quote-----
       
       мне кажется имелось ввиду "но она", нелепая опечатка...
       это в качестве направления к достижению 8)

     email: "dont@avail.able"

  -  author: "akella"
     id: "3327"
     url: "http://cssing.org.ua"
     date: "2006-05-24 20:25:55"
     humandate: "24 May, 2006"
     content: | 
       Спасибо исправил.

     email: "akella.a@gmail.com"

layout: "layouts/post.njk"
excerpt: "Долго не писал в блог - очень мало времени - потом понял, что все время искал нечто глобальное и большое. Теперь стратегию решил изменить, буду теперь писать чаще и мельчее. )

Маленький трик с посещенными ссылками для \"хороших\" броузеров.
<strong>Update</strong>: дал маху - об этом уже написали <a href=\"http://www.umade.ru/log/2005/09/110.html\">Посещенные ссылки. Visited links</a> - на Юмэйд. Ничего не воровал - просто дал маху :(.
"
---

Долго не писал в блог - очень мало времени - потом понял, что все время искал нечто глобальное и большое. Теперь стратегию решил изменить, буду теперь писать чаще и мельчее. )

Маленький трик с посещенными ссылками для "хороших" броузеров.
<strong>Update</strong>: дал маху - об этом уже написали <a href="http://www.umade.ru/log/2005/09/110.html">Посещенные ссылки. Visited links</a> - на Юмэйд. Ничего не воровал - просто дал маху :(.
<!--more-->
<h3>Ставим галочки</h3>
Один из способов красиво выделить посещенные ссылки не используя картинки. Ближе к делу:
<ol class="code">
<li>a:visited:after {</li>
<li class="tab">content:"\00A0\2713";</li>
<li>}</li>
</ol>
Или так (так делает Майк Дэвидсон у себя на сайте - разницу будет трудно увидеть ):
<ol class="code">
<li>a:visited:after {</li>
<li class="tab">content: "\00A0\221A";</li>
<li class="tab">font-size: 75%;</li>
<li>}</li>
</ol>
Псевдокласс :after работает уже практически везде (кроме сами знаете кого ;)). Таким образом во всех(!ИЕ) броузерах посещенные линки выделятся примерно таким образом(картинки в порядке CSSов):

<img src="/images/rad1.gif" title="Roger Johansson метод" alt="Roger Johansson метод" /><img src="/images/rad2.gif" title="Mike Davidson метод" alt="Mike Davidson метод" />

Вот такие красивые радикальчики-галочки. Среди символов есть и настоящая "галочка" (check mark) - но она, к сожалению, отображается далеко не во всех броузерах..
Если указывать символы не в юникоде, возникают проблемы c броузерами - посему все в таком неочевидном на первый взгляд виде. Однако же работает. А ИЕ... это его проблемы ;)

Вот такой маленький прием - вид конечно на любителя - но я думаю применение не настолько надуманное. Мне лично, очень даже нравится. Если в свободное время я выиграю "бой с ленью" то и себе такие сделаю :).
<h3>Ссылки по теме</h3>
<ul>
<li><a href="http://www.456bereastreet.com/archive/200509/check_marking_visited_links/">Check marking visited links</a>  - собственно эту заметку я перевел</li>
<li><a href="http://icant.co.uk/csstablegallery/index.php?css=36">Пример первого CSS кусочка</a></li>
<li><a href="http://www.mikeindustries.com/blog/archive/2004/06/radical-links">Майк Дэвидсон про этот же маленький прием - у него на сайте живой пример второго кусочка CSS</a></li>
<li><a href="http://www.unicode.org/charts/">Символы юникода</a></li>
<li><a href="http://www.digitalmediaminute.com/reference/entity/index.php">XHTML символы</a> - красиво и удобно</li>
<li><a href="http://www.collylogic.com/index.php?/weblog/comments/ticked_off_links_reloaded/">Более "продвинутый" вариант</a> - с картинками, а не радикалами</li>
</ul>
