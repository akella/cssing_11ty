---
title: "Настоящий XHTML или пока не стоит?"
date: "2005-02-25"
humanDate: "25 Feb, 2005"
permalink: "2005/02/25/xhtml-worth-or-not/"
tags: 
  - "xhtmlcss"
comments: 
  -  author: "Dmitry"
     id: "897"
     url: "http://www.webstylestudio.com"
     date: "2005-03-08 16:46:30"
     humandate: "08 Mar, 2005"
     content: | 
       :-)
       
       Как раз я и спорил с Вами!
       
       Опять-таки - w3c и разработчики современных броузеров говорят - application/xhtml+xml
       
       Для совместимости использовать content negotiation. Note: это не джаваскипт, как указано выше ;-)
       
       Без application/xhtml+xml сайт парсится как HTML, те есть настоящим HTML 4 + закрытые теги + теги маленькими буквами + все атрибуты в кавычках. Если же используется application/xhtml+xml сайт парсится как XML. А вот если мы почитаем спецификацию по XHTML даже первой версии - там указано что XHTML это XML (прим. - а не HTML).
       
       Поэтому это ошибка не использовать правильный mime!
       
       Тем более уже есть официальная спецификация XHTML 1.1 и я надеюсь скоро будет XHTML 2. Где, к вашему сожалению и речи не будет о mime типа text/html.
       
       Те мое мнение - Вы сделали правильный шаг вперед но остановились все еще на HTML (или как говорит w3c - совместимый XHTML, но не XHTML по его назначению, те никаких преимуществ).
       
       Вот так вот! ;-)

     email: "yeskin@webstylestudio.com"

  -  author: "akella"
     id: "898"
     url: "http://cssing.iatp.org.ua"
     date: "2005-03-08 16:55:37"
     humandate: "08 Mar, 2005"
     content: | 
       http://www.webmascon.com/topics/technologies/11a.asp
       2000 год акценты сменились но суть осталась...
       К сожалению мнение в3ц(хотя скорее ваше его толкование) для меня не так авторитетно.

     email: "akella.a@gmail.com"

  -  author: "ganges"
     id: "865"
     url: "http://development.it.net.ua"
     date: "2005-03-04 14:37:00"
     humandate: "04 Mar, 2005"
     content: | 
       "Грубой ошибкой" является только при использовании XHTML 1.1 при
       использовании XHTML 1.0 даже Strict является допустимым
       Критик пусть читает спецификацию и <a href="webstandards.org">webstandards.org</a>

     email: "andrey.stefanenko@gmail.com"

  -  author: "Yukki Pospel"
     id: "772"
     url: "http://blog.emo.com.ua"
     date: "2005-02-26 03:08:23"
     humandate: "26 Feb, 2005"
     content: | 
       По-моему этому "разработчику" не дают покоя собственные амбиции и желание поучать других. Если я правильно понял о ком идет речь ;)

     email: "creative@emo.com.ua"

  -  author: "akella"
     id: "773"
     url: "http://cssing.iatp.org.ua"
     date: "2005-02-26 13:09:51"
     humandate: "26 Feb, 2005"
     content: | 
       Абсолютно правильно. :)
       Но тем не менее подобный спор имел место и в веб-стандартном сообществе вообще. Поэтому мне было бы интересно узнать мнение и нашей мафии по этому вопросу.

     email: "akella.a@gmail.com"

  -  author: "Yukki Pospel"
     id: "774"
     url: "http://blog.emo.com.ua"
     date: "2005-02-26 13:42:54"
     humandate: "26 Feb, 2005"
     content: | 
       Спор спором, но совесть тоже надо иметь.
       
       На счет content-type мое мнение такое - использование html/text не нарушает стандарты и оправданно реалиями времени. Если уж на то пошло, html 4.01 тоже подмножество XML и с точки зрения такое логики может быть отнесен к application/xml. Как правильно заметил Майк Дэвидсон ломать тут копья не обо что - это дело сугубо личное что выбирать на этом этапе, так как многие аспекты должны быть учтены (главные ты лаконично и ясно описал). А в будущем надо быть готовым сделать код более "стандартным".
       
       Техническое совершенство страниц и их дизайн-исполнение суть разные аспекты разработки.

     email: "creative@emo.com.ua"

  -  author: "ilya shvets"
     id: "787"
     url: "http://witness.dp.ua"
     date: "2005-02-28 10:26:02"
     humandate: "28 Feb, 2005"
     content: | 
       Света не было,.. : (
       Как результат - в ближайшее время планируем перенести хост-площадку в гермозону Укртелеома. Они вроде неплохо работать стали в последнее время.

     email: "shvets@gmail.com"

  -  author: "Vladson"
     id: "827"
     url: "http://dkflbk.nm.ru/"
     date: "2005-03-03 02:50:38"
     humandate: "03 Mar, 2005"
     content: | 
       А что мешает вставить в скрипт (в РНР например) ?
       header('Content-Type: application/xhtml+xml; charset=utf-8');

     email: "vladson@heatpc.com"

  -  author: "Vladson"
     id: "828"
     url: "http://dkflbk.nm.ru/"
     date: "2005-03-03 02:56:28"
     humandate: "03 Mar, 2005"
     content: | 
       ААА вдуплил, IE не открывает его

     email: "vladson@heatpc.com"

  -  author: "Dmitry"
     id: "899"
     url: "http://www.webstylestudio.com"
     date: "2005-03-08 18:39:57"
     humandate: "08 Mar, 2005"
     content: | 
       2000 год тогда и броузеров то толковых не было ;-)
       
       Вот вам ответ из w3c FAQ:
       http://www.w3.org/MarkUp/2004/xhtml-faq.html#texthtml
       ключевая фраза не та что это разрешается из-за того что разработчики броузеров постарались в совместимости, а та что: "be well aware, sending XHTML documents to browsers as text/html means that those browsers see the documents as HTML documents, not XHTML documents."
       
       И не надо здесь ссылок тулить тем более 2000 года - мне просто в лом искать ссылки на не менее авторитетные статьи - я акелле показывал (например от разработчика оперы).
       
       там же есть про то что XHTML1.1 не может быть ни в коем случае размещен как text/html

     email: "yeskin@webstylestudio.com"

  -  author: "Dmitry"
     id: "901"
     url: "http://www.webstylestudio.com"
     date: "2005-03-09 11:48:16"
     humandate: "09 Mar, 2005"
     content: | 
       А вообще суть то не в том что Вам кто-то запрещает или разрешает использовать text/html. Я не об этом спорю. Если хотите используйте дальше это Ваше право. Суть в том, что при text/html у вас HTML, а не XHTML. Это я и пытался доказать.

     email: "yeskin@webstylestudio.com"

  -  author: "Dmitry"
     id: "902"
     url: "http://www.webstylestudio.com"
     date: "2005-03-09 11:50:40"
     humandate: "09 Mar, 2005"
     content: | 
       А что касается расширяемости то ВЫ сможете использовать не только MathML, а и SVG, SMIL, xForms (очень мощная штука но пока мало кем поддерживается), а также кучу других XML-совместимых технологий.
       
       ;-)

     email: "yeskin@webstylestudio.com"

  -  author: "akella"
     id: "903"
     url: "http://cssing.iatp.org.ua"
     date: "2005-03-09 11:54:37"
     humandate: "09 Mar, 2005"
     content: | 
       Ключевое слово
       <strong>мало кем поддерживается</strong>
       Я б сказал НИКЕМ. Даже у ФФ нужно качать отдельные версии...

     email: "akella.a@gmail.com"

  -  author: "Aleks Khodalev"
     id: "983"
     url: "http://www.creativepro.ru"
     date: "2005-03-18 16:33:19"
     humandate: "18 Mar, 2005"
     content: | 
       to Dmitry
       
       Cделайте, что-то сами. И покажите как это все прекрасно работает...
       А то заходишь к вам на сайт и видишь верстку образца 96 года.

     email: "akh@creativepro.ru"

  -  author: "ganges"
     id: "1415"
     url: ""
     date: "2005-04-14 12:41:34"
     humandate: "14 Apr, 2005"
     content: | 
       А вот валидатор говорит text/html
       
       A FF говорит "application/xhtml-xml" (!!!!-SIC-!!!!)
       
       Feed валидатор говорит
       This feed does not validate.
        Feeds should not be served with the "text/html;charset=utf-8" media type"
       
       Дмитрий, ты че нас совсем за лохов держишь? Издеваешься, да?
       
       Валидатор, к твоему сведению отлично "хавает" и хидеры и правильный медиа-тайп. Поэтому если действительно application, то он и пишет - "application/xhtml+xml" ! Заметь, ПЛЮС XML, а не МИНУС, как у тебя :))) [05.04.14] Сам себя выдешь, чистый Фрейд.
       
       application/xhtml-xml НЕТ ТАКОГО медиа-тайпа
       
       А это значит, что ты его "вручную" подставляешь, я вот только не понимаю зачем? Чтобы рассказать здесь, что ЭТО "правильный" XHTML? Но эту пургу можно втирать своим клиентам, а не пацанам, читающим CSSing. :)

     email: "andrey.stefanenko@gmail.com"

  -  author: "Dmitry"
     id: "1157"
     url: "http://www.webstylemedia.com"
     date: "2005-03-29 12:51:47"
     humandate: "29 Mar, 2005"
     content: | 
       сорри то местный сайт. Но те кто меня знают в курсе что мы XHTML делаем с правильным размещением. есть еще вот такой вот:
       http://www.webstylemedia.com
       
       на нем кстати обратите внимание что используется application/xhtml+xml, а все javascript -ы используют DOM. И никаких проблем нет (правда мы там стилями перегрузили его сильно - но это не нарушение стандарта)
       
       Успехов!

     email: "yeskin@webstylestudio.com"

  -  author: "akella"
     id: "1189"
     url: "http://cssing.iatp.org.ua"
     date: "2005-03-31 09:31:28"
     humandate: "31 Mar, 2005"
     content: | 
       Да я вижу это часть вашего стиля писать 5 строк ЦСС там где можно одной обойтись... :) И по фудкомпонент видно было...
       А вот проблема с отображением в Мозилле как раз есть. Сайт отображается лишь после полной загрузки файла. Что ИМО не есть хорошо.
       Скромно замечу, не сочтите придиркой, но сайт в портфолио не относится к слову веб-стандарты. Скорее наоборот.

     email: "akella.a@gmail.com"

  -  author: "Dmitry"
     id: "1209"
     url: "http://www.webstylemedia.com"
     date: "2005-04-01 16:10:19"
     humandate: "01 Apr, 2005"
     content: | 
       :-)
       
       Насчет 5-ти строк - ты имеешь ввиду сделать импортом? У меня есть личное мнение на этот счет - хотя я могу ошибаться - иногда на сайтах с импортом стилей нельзя сохранить страницу в эксплорере - те сохранить полностью - происходит глюк эксплорера. Поэтоу лучше написать проще пятьми строками. Хотя это лишь мое мнение и оно может быть некорректным.
       
       Насчет сайта в портфолио - да согласен но фудкомпанент явно не катит под портфолио американской компании. Хотя в будущем там будут только сайта с веб-стандартами. Там вообще пока портфолио не наполнено хотя оно есть.

     email: "yeskin@webstylestudio.com"

  -  author: "Dmitry"
     id: "1210"
     url: "http://www.webstylemedia.com"
     date: "2005-04-01 16:12:01"
     humandate: "01 Apr, 2005"
     content: | 
       Собственно по этой причине я этот сайт и не показывал.... ;-)

     email: "yeskin@webstylestudio.com"

  -  author: "akella"
     id: "1211"
     url: "http://cssing.iatp.org.ua"
     date: "2005-04-01 16:23:34"
     humandate: "01 Apr, 2005"
     content: | 
       Да нет я имел ввиду что вместо
       <ol class="code">
       <li>padding-top: 6px;</li>
       <li>padding-bottom: 4px;</li>
       <li>padding-left: 30px;</li>
       <li>pading-right: 17px;</li>
       </ol>
       Можно писать <ol class="code"><li>padding:6px 17px 4px 30px;</li></ol> Только и всего. Складывается впчатление что ЦСС генерируется а не пишется. Вот и все что я имел ввиду.

     email: "akella.a@gmail.com"

  -  author: "Dmitry"
     id: "1212"
     url: "http://www.webstylemedia.com"
     date: "2005-04-01 16:30:41"
     humandate: "01 Apr, 2005"
     content: | 
       это знаю.... 
       оптимизировать CSS конечно можно и нужно и это сделаем позже...
       просто такие вещи получались именно в момент исправления визуальных ошибок и в итоге получилось такое награмождение... Но опять-таки я некомментирую код или цсс внутри укр нета - не вижу смысла продолжать попытки найти ошибки и недостатки - их можно найти всегда. Я просто говорил и говорю что сайты должны быть размещены как application/xhtml+xml иначе получается не XHTML. ;-)
       
       Кстати вскоре мы попробуем добавить спецефические вещи - такие как xForms, SVG, SMIL, xInclude (возможно).

     email: "yeskin@webstylestudio.com"

  -  author: "akella"
     id: "1213"
     url: "http://cssing.iatp.org.ua"
     date: "2005-04-01 16:34:57"
     humandate: "01 Apr, 2005"
     content: | 
       Вот и отлично.
       Будет очень интересно посмотреть на все преимущества.
       
       Да о чем вы говорите мне абсолютно неинтересно упрекать кого-либо в чем-либо. Мне лишь было любопытно: почему не сокращаете.

     email: "akella.a@gmail.com"

  -  author: "Dmitry"
     id: "1775"
     url: "http://www.webstylemedia.com"
     date: "2005-05-24 14:41:45"
     humandate: "24 May, 2005"
     content: | 
       Вы чего? Сайт размещен как раз таки на xhtml+xml. Это наш SEO который с мета тагами работал - добавил xhtml-xml в мета контент тайп. Но миме как раз таки был xhtml+xml (миме на сервере). Это вы меня за лоха не держите! Все как раз в норме.
       
       что касается фидов то там несколько сложнее - мы не выкладываем фиды как обычный xml файл. Мы формируем фиды динамически и выдаем их как файл для скачивания причем с нужным миме. Валидатор такого не хавает.
       
       Вот так вот.

     email: "info@webstylemedia.com"

  -  author: "Артём"
     id: "4016"
     url: "http://jobmarket.com.ua"
     date: "2006-07-21 16:07:56"
     humandate: "21 Jul, 2006"
     content: | 
       100% согласен с автором. Спасибо

     email: "anydasa@mail.ru"

  -  author: "bw"
     id: "9911"
     url: "http://www.handsdriver.net/"
     date: "2007-03-22 04:55:03"
     humandate: "22 Mar, 2007"
     content: | 
       По недостаткам, которые перечислил автор:
       1. Это зависит от реализации браузера, HTML не менее структурированным документом чем XML, но тем не менее его научились отображать частично.
       2. Невижу проблем. Используйте DOM. Я программист. И мне такой подход кажется более правильным, возможно, немного сложнее чем write, но это только до первого типового решения.
       3. Кривые руки разработчика. При наличии ошибок каждый браузер будет испралять их по своему в следствии чего конечный результат на разных браузерах будет разным.
       4. Не вижу сложностей. Т.е. я наверное не очень понимаю о чем речь.
       5. JS не нужен. Но на это уже был ответ.
       
       Единственный серьезный недостаток заключается в том что сейчас "самый лучший браузер" не работает с XHTML, следовательно теряются все его преимущества над HTML (те преимущества что нужны конечному пользователю).

     email: "bw@handsdriver.net"

  -  author: "akella"
     id: "9955"
     url: "http://cssing.org.ua"
     date: "2007-03-22 15:49:18"
     humandate: "22 Mar, 2007"
     content: | 
       Доводы разумны, но абстрактны,
       1. На данный момент основные браузеры реализованы именно так. Де факто. (а ведь со времени поста прошло больше 2х лет, может... в следующем году?=))
       2. Да, безусловно вы правы, но скажите это царству баннеров и информеров рунета и юанета, это неправильно но это большая проблема. Возьмите хоть яндекс директ, вот и все...
       3. тем не менее именно так на данный момент обрабатываются ошибки в коде для XML и XHTML, факт, не самый приятный для пользователя и требует массы усилий по обезопасиванию кода, если речь идет не о 1001 вордпресс блоге.
       4. Повторение пункта про баннеры и информеры
       5. Джс или ПХП нужен, если вы не хотите работать с ИЕ в квиркс моуде. А это вобщем то нормально как по мне.

     email: "akella.a@gmail.com"

  -  author: "Я"
     id: "11088"
     url: "http://egorod.com/"
     date: "2007-07-19 19:32:10"
     humandate: "19 Jul, 2007"
     content: | 
       Я считаю что автор по большей части всетаки прав, хотя.... есть некоторые оговорки о которых можно было бы долго поговорить

     email: "sdf@ya.com"

  -  author: "Rich"
     id: "11863"
     url: ""
     date: "2008-02-27 11:09:49"
     humandate: "27 Feb, 2008"
     content: | 
       Однажды столкнулись с такой проблемой.
       Решение простое - проверять с какого домена(или ip) запрашивают страничку - если с validator.w3.org - выдавать контент тайп xhtml+xml :)

     email: "bill-gates@ukr.net"

layout: "layouts/post.njk"
excerpt: "<strong>Не по теме:</strong> Эхх... Хостинг упал на целых два дня... :( Сорри всем кто пытался.

Недавно меня уличили в том что страничка <a href=\"http://www.ukr.net/\">UkrNet</a> не то что не удовлетворяет стандарту <abbr title=\"eXtensible Hypertext MarkUp Language\">XHTML</abbr>. А самым грубейшим образом его нарушает. И вообще немедленно должна быть отредактирована.
Первая мысль была \"хм?!\" - валидатор говорит ок!, и наличествует грубая ошибка.
"
---

<strong>Не по теме:</strong> Эхх... Хостинг упал на целых два дня... :( Сорри всем кто пытался.

Недавно меня уличили в том что страничка <a href="http://www.ukr.net/">UkrNet</a> не то что не удовлетворяет стандарту <abbr title="eXtensible Hypertext MarkUp Language">XHTML</abbr>. А самым грубейшим образом его нарушает. И вообще немедленно должна быть отредактирована.
Первая мысль была "хм?!" - валидатор говорит ок!, и наличествует грубая ошибка.
<!--more-->
<h3>А дело было вот в чем</h3>
Есть такой не совсем давний спор под названием "content negotiation".
Заключается она вот в чем.
Согласно рекомендации <abbr title="eXtensible Hypertext MarkUp Language">XHTML</abbr> сама страничка удовлетворяющая этому стандарту должна подаваться как "<strong>text/xml, application/xml, или application/xhtml+xml</strong>" . однако так же обозначается что он(контент тайп) может быть <strong>text/html</strong>.
Так вот это и было засчитано как грубейшая ошибка, несмотря на то что валидатор её "для простоты" игнорирует.
<h3>В чем разница</h3>
А разница состоит в том, что при указании правильного контент тайпа(xhtml+xml) Опера и ФФ используют другой парсер для отображения. Который работает быстрее.
Второе отличие, что в результате мы получаем не так называем "<strong>tag soup</strong>" то есть кашу из тэгов или обычный <abbr title="Hypertext MarkUp Language">HTML</abbr>, а <abbr title="eXtensible Hypertext MarkUp Language">XHTML</abbr> то есть почти XML.
В конце я приведу несколько ссылок, а пока сделаю свои выводы, если в чем то неправ поправьте в комментах:
<dl>
<dt>Итак сначала что мы выигрываем от использования правильного ДТД</dt>
<dd><ul style="margin:0;padding:0;"><li>Мы получем "расширяемость"  <abbr title="eXtensible Hypertext MarkUp Language">XHTML</abbr>, то есть можем использовать другие ДТД типа MathML прямо в XHTML коде. Но для укрнет это пока что мягко говоря излишне</li>
<li>Странички будут рендерится быстрее, но только у ФФ и Оперы.
(рендерится значит сам броузер будет обрабатывать изображение с большей скоростью) но не грузиться быстрее.</li>
<li>Наконец у нас выйдет не тэг суп а настоящий XHTML (ура?!)</li>
<li>Это круто, это  стандарт, это будущее</li>
</ul>
</dd>
<dt>А теперь недостатки</dt>
<dd>
<ul style="margin:0;padding:0;"><li>страничка будет отображаться только после полной загрузки
файла.(юзер икспириенс и хиты вниз)</li>
<li> множество джаваскриптов перестает работать (типа документ.врайт) - надо переписывать заново.</li>
<li> при наличии ошибок страничка не будет отображена вообще(в опере и ФФ).</li>
<li> сложности с подгонкой динамического кода под такой строгий стандарт</li>
<li>необходимость вставки в Хед файла ДЖскрипта который разным броузерам будет "записывать" разные ДТД. И совсем не факт что правильно.(ИЕ не понимает правильного доктайпа)</li>
</ul>
</dd>

</dl>
Вобщем в целом ни броузерный рынок (ИЕ попросту не понимает xhtml+xml) ни сам стандарт ИМХО еще не готовы для повсеместного внедрения.
Вот из таких предпосылок я и решил не переходить на данный контен тайп.

Однако после этого возникает вопрос: почему я использую доктайп XHTML 1.0?
Действительно <strong>формально</strong>  у меня всего лишь обычный HTML и никак не XHTML.
Однако я считаю для себя правилом употреблять кавычки для всех атрибутов, писать их с маленькой буквы, закрывать одиночные тэги и так далее. Валидатор же при доктайпе HTML, не найдет даже таких простых ошибок.
И к тому же я считаю что само W3C позволяет использовать такой способ подания XHTML как переходной вариант. Ведь сами броузеры еще к нему не совсем готовы.

Собственно этот пост вылился из спора с одним веб-разработчиком, который почему то считает это(контент тайп на укр.нет) грубой ошибкой.
Вот ресурсы где можно подробнее узнать об этом споре:
<ul>
<li><a href="http://www.autisticcuckoo.net/archive.php?id=2004/11/03/content-negotiation">Content Negotiation</a></li>
<li><a href="http://blog.deconcept.com/2004/11/03/why-its-ok-to-send-xhtml-as-text-html/">Why it’s OK to send XHTML as text/html</a> - здесь очень много комментариев, среди прочих и Майк Дэвидсон отметился...</li>
<li><a href="http://www.spartanicus.utvinternet.ie/no-xhtml.htm">No to XHTML</a></li>
</ul>

<strong>ЗЫ</strong>: в следующей заметке напишу о глюках что я выловил во время разработки <a href="http://www.ukr.net/">Ukr.Net</a>
