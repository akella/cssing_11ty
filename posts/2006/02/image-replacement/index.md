---
title: "Некоторые техники замены текста картинками (image replacement)"
date: "2006-02-23"
humanDate: "23 Feb, 2006"
permalink: "2006/02/23/image-replacement/"
tags: 
  - "xhtmlcss"
  - "design"
comments: 
  -  author: "Flack"
     id: "2795"
     url: "http://flack.ru"
     date: "2006-02-23 14:53:24"
     humandate: "23 Feb, 2006"
     content: | 
       Спасибо, Thierry Image (re)Placement пока не встречал. Обязательно попробую.

     email: "alex@flack.ru"

  -  author: "ganges"
     id: "2796"
     url: "http://idcontent.com/"
     date: "2006-02-23 15:37:46"
     humandate: "23 Feb, 2006"
     content: | 
       Я делаю так. 
       
       h1 {
       	height:80px;
       	width:200px;
       	background:#fff url(someimage.gif);
       	}
       	h1 span {
       	display:none;
       	}
       	
       И HTML
       
       	&lt;h1&gt;&lt;span&gt; Заголовок - картинка &lt;/span&gt;&lt;/h1&gt;
       	
       Конечно, при выключенных картинках и включенном CSS не видно ничего. Это наверное самый примитивный IR. А вообще я за CSS3 метод :)

     email: "andrey.stefanenko@gmail.com"

  -  author: "Kildor"
     id: "2797"
     url: "http://opera.nsk.su"
     date: "2006-02-23 17:39:06"
     humandate: "23 Feb, 2006"
     content: | 
       Кстати, Опера давно уже поддерживает CSS3 метод ;-)

     email: "kostia@ngs.ru"

  -  author: "akella"
     id: "2798"
     url: "http://cssing.org.ua"
     date: "2006-02-23 18:14:54"
     humandate: "23 Feb, 2006"
     content: | 
       коммент на правах рекламы :)

     email: "akella.a@gmail.com"

  -  author: "MAX"
     id: "2800"
     url: "http://mysevastopol.com/"
     date: "2006-02-23 23:43:00"
     humandate: "23 Feb, 2006"
     content: | 
       А я пробовал «Header Image Generator» :) (http://www.alistapart.com/articles/dynatext/) Работает на ура. Главное ttf-шрифт на сервер закачать :)

     email: "max-3000@list.ru"

  -  author: "uggallery"
     id: "2802"
     url: "http://uggallery.audiopeace.ru"
     date: "2006-02-26 19:36:12"
     humandate: "26 Feb, 2006"
     content: | 
       Странно, что нет методов (мне не попадались) вроде LIR-a, но где для сокрытия текста используются манипуляции с line-height. Это работает даже в IE 5.0. Правда, проверял не во всех браузерах. На маке, например, не проверял. Может есть какие-то противопаказания?

     email: "uggallery@yandex.ru"

  -  author: "akella"
     id: "2803"
     url: "http://cssing.org.ua"
     date: "2006-02-27 12:39:58"
     humandate: "27 Feb, 2006"
     content: | 
       А как именно с помощью лайн-хейт Вы предлагаете?
       очень большой или очень маленький? или отрицательный? Я как то и сам не пробовал - хотя и заметно что можно текст наверно смещать сильно по вертикали. Можно чуть подробнее?

     email: "akella.a@gmail.com"

  -  author: "ganges"
     id: "2804"
     url: "http://idcontent.com/"
     date: "2006-02-27 12:51:45"
     humandate: "27 Feb, 2006"
     content: | 
       http://meyerweb.com/eric/thoughts/2006/02/08/unitless-line-heights/
       
       Что меня лично наводит на мысль о том, что гипотетический метод IR с помощью line-height - не самый лучший. Я наступал на грабли с этим проперти в более простейшей ситуации, чем IR.
       Отрицательный не покатит, ИМХО :)

     email: "andrey.stefanenko@gmail.com"

  -  author: "akella"
     id: "2805"
     url: "http://cssing.org.ua"
     date: "2006-02-27 14:15:04"
     humandate: "27 Feb, 2006"
     content: | 
       Не совсем понял кстати параллель? Там же просто в очередной раз написали что лайн-хейт можно без единиц употреблять? А как это связано с граблями при ее употреблении?

     email: "akella.a@gmail.com"

  -  author: "uggallery"
     id: "2806"
     url: "http://uggallery.audiopeace.ru"
     date: "2006-02-27 17:37:41"
     humandate: "27 Feb, 2006"
     content: | 
       <a href="http://uggallery.narod.ru/line-height-ir/" rel="nofollow">Test-case для проверки/</a> 
       
       Похоже, line-height c большим значением работает в самых популярных браузeрах. Нулевой -- так-сяк, а отрицательный не работает вообще. Но реальность, конечно, может оказаться сложнее.

     email: "uggallery@yandex.ru"

  -  author: "ganges"
     id: "2807"
     url: "http://idcontent.com/"
     date: "2006-02-27 17:47:28"
     humandate: "27 Feb, 2006"
     content: | 
       А можно и с единицами :) Konqueror в моей разметке без едениц выдавал "страшную байду", а с еденицами - все ок. Я, ясное дело сначала без едениц написал - пропустил через валидатор - а он - "говно мол, не катит". Если бы тут Мейер свою заметку не написал, я бы наверное волосы на голове порвал :) Во как бывает
       
       Паралель в том.что эксперимантировать с line-height с такой "скользкой" техникой как IR я считаю потенциально багоопасным.
       
       На конкверор, конечно, можно забить, если забыть, что это "почти Safary"

     email: "andrey.stefanenko@gmail.com"

  -  author: "uggallery"
     id: "2808"
     url: "http://uggallery.audiopeace.ru"
     date: "2006-02-27 17:57:13"
     humandate: "27 Feb, 2006"
     content: | 
       &gt;считаю потенциально багоопасным
       
       Согласен. Хотя любой IR "багоопасен", любой требует проверки. А этот, видимо, очень неплохо подходит для пятого IE, чем и привлекает.

     email: "uggallery@yandex.ru"

  -  author: "UGgallery -Замещение текста с помощь..."
     id: "2809"
     url: "http://uggallery.audiopeace.ru/2006/02/27/line-height-ir"
     date: "2006-02-27 19:05:45"
     humandate: "27 Feb, 2006"
     content: | 
       [...] Есть идея использовать для замещения текста (image replacement) CSS-свойстов line-height. Идея требует проверки, но уже сейчас кажется вполне перспективной [...]

     email: ""

  -  author: "uggallery"
     id: "2811"
     url: "http://uggallery.audiopeace.ru"
     date: "2006-02-27 19:24:16"
     humandate: "27 Feb, 2006"
     content: | 
       Эх! В 5.5-то я и не проверил :( До чего ж они разные эти IE. А я это уже в одном эскизе использовал. Пойду исправлять на _line-height:0 или что-нибудь в этом роде. Спасибо.

     email: "uggallery@yandex.ru"

  -  author: "akella"
     id: "2810"
     url: "http://cssing.org.ua"
     date: "2006-02-27 19:07:04"
     humandate: "27 Feb, 2006"
     content: | 
       Да - оперативно сработал :)
       
       Это малозначимо - но вообще как факт - сначала случайно запустил 5.5 а не 5.01 - и при большом позитивном line-height - сверху от элемента соответствующее пустое пространство - чего, однако, не наблюдается в других ИЕ. Пожалуй letter-spacing в этом смысле чуть более универсален. Хотя как вариант - нулевой лайн хейт можно отдавать ИЕ безболезненно.
       То бишь например вариант сочетания LIR (самый первый в посте и не работающий в ИЕ 5.0) очень даже привлекателен:
       <strong>_line-height:0;</strong>

     email: "akella.a@gmail.com"

  -  author: "Арки"
     id: "3216"
     url: "http://marpa.narod.ru/"
     date: "2006-05-15 16:09:00"
     humandate: "15 May, 2006"
     content: | 
       CSS-хаки - это круто, конечно, но с выходом ИЕ 7 будут большие проблемы. Опять придется переделывать все сайты.
       
       Да и тестирование сайта во всех версиях ИЕ: 4, 5.0, 5.01, 5.5, 6.0, 7.0, а еще Файрфоксы, Оперы, Сафари, Konqueror - немножко напрягает.
       
       Может, перестать изобретать велосипед, и просто оставить "по умолчанию" - чтобы весь текст выводился тем шрифтом, который указан в браузере (Times New Roman). Или выбрать Verdana - он выглядит гораздо лучше.
       
       Но вот что мне не нравится - когда текст на сайте фиксированного размера. Читать неудобно! А разве текст не предназначен для чтения? 
       
       Я, конечно, знаю, как избавиться от фиксации размера шрифта в браузере, но при этом вся DIV-ная верстка жутко разъезжается, куски текста переплетаются, блоки перекрывают друг друга или уходят вниз. Получается нечитабельная помойка.
       
       Совет: всегда проверяйте вид сайта при маленьком разрешении и с большим размером шрифта - узнаете много дового о верстке.
       
       В общем, по-прежнему действует правило: хочешь сделать крутой современный сайт с наворотами, верстай DIV-ами и с большим количеством CSS. Хочешь быстро сделать простой и удобный сайт - делай табличную верстку с минимумом CSS.

     email: "marpa@narod.ru"

  -  author: "akella"
     id: "3221"
     url: "http://cssing.org.ua"
     date: "2006-05-15 20:51:54"
     humandate: "15 May, 2006"
     content: | 
       У Вас получился замечательный монолог, строго подтверждающий Вашу правоту. :)
       
       Но во первых никаких особенно страшных проблем с ИЕ 7 я не вижу пока что. А если учесть что до его выхода еще полгода. ТО об этом думать пока все же рано.
       
       Во вторых если оно разьезжается значит сайт сверстан плохо. В идеале должно расширяться. И я в данном случае подаю плохой пример. Но это отнюдь не камень в сторону правильной верстки. В данном случае она ничем не отличается от табличной.
       
       Совет - очень хороший :). В таком случае всегда проверяйте ваши сайты натаблицах мобильниками, поисковиками(на предмет кучи лишнего кода), принтерами на предмет печатных версий ит д. Узнаете еще больше нового.
       
       А правило боюсь действует для Вас. :) Но никак не для меня. 
       Вы напоминаете крестьянина который ворчит на трактор и говорит - "да проще лопатой вскопать, чем трактор заводить, бензин заливать"... :)

     email: "akella.a@gmail.com"

  -  author: "akella"
     id: "3374"
     url: "http://cssing.org.ua"
     date: "2006-05-27 10:30:37"
     humandate: "27 May, 2006"
     content: | 
       Порообуй писать тот ЦСС для замены текста на картинку не для "h1", а для "h1 a". Добавив туда правило <strong>display:block</strong>
       Должно получиться.

     email: "akella.a@gmail.com"

  -  author: "Shimon"
     id: "3356"
     url: ""
     date: "2006-05-26 14:46:28"
     humandate: "26 May, 2006"
     content: | 
       Все прекрасно, только у меня почему то в первом способе никак не удается валидно приделать ссылку на заголовок :'(
       
       а span как то не хочется...

     email: "shimonenator@gmail.com"

  -  author: "Максим Вуец"
     id: "3475"
     url: ""
     date: "2006-06-03 13:44:42"
     humandate: "03 Jun, 2006"
     content: | 
       Может я чего не понимаю, но почему не проще сделать так:
       h1 span { display: none; }
       &lt;h1&gt;
       &lt;span&gt;title&lt;/span&gt;
       &lt;img src=&quot;img.gif&quot;/&gt;
       &lt;/h1&gt;

     email: "m-by@ya.ru"

  -  author: "Ivan A-R"
     id: "3496"
     url: "http://iar.spb.ru"
     date: "2006-06-06 18:36:48"
     humandate: "06 Jun, 2006"
     content: | 
       Да. Вроде как через скрытие логичнее получается. У меня картинка на заголовок полупрозрачная, и я сделал так:
       
       h1 {
       height:85px; width:700px;
       	overflow:hidden;
       	background: transparent url("images/title.gif") no-repeat;
       }
       h1 span {
       	visibility: hidden;
       }
       
       title
       
       Где грабли выплывут?

     email: "plumbum@rambler.ru"

  -  author: "akella"
     id: "3497"
     url: "http://cssing.org.ua"
     date: "2006-06-06 21:28:30"
     humandate: "06 Jun, 2006"
     content: | 
       Все зависит от задач которые вы ставите перед собой. К примеру - ПРОСТО надо заменить нечто на картинку - без заморочек с аксессабилити и тд - мне было бы стыдно добавлять СПАН я бы сделал без него.
       Другой вариант - нужно заморочится на аксессабилити - то есть что бы как минимум с отключенными картинками показывало текст какой то хоть. Но тогда твой метод Иван не подходит.
       
       С другой стороны что лично мне иногда претило бы использовать метод Максима - та картинка на которую я заменяю текст - иногда служит все же частью дизайна и лучше ей быть в фоне. + контент дублируется. Но для других случаев совсем не плохой вариант. У Тьерри некое подобие такого подхода - <a href="http://www.tjkdesign.com/articles/tip.asp" rel="nofollow">Thierry Image Placement</a>.
       Короче чаще зависит от конкретного случая - иногда чего уж греха таить можно и влепить пустой див, пока никто не видит и потом не спать ночами от угрызений совести. только так :)

     email: "akella.a@gmail.com"

  -  author: "Ivan A-R"
     id: "3521"
     url: "http://iar.spb.ru"
     date: "2006-06-09 12:46:27"
     humandate: "09 Jun, 2006"
     content: | 
       Спасибо. Я уже потом допёр, что с отключёнными картинками заголовка не будет.
       
       Опять же, я исходил из того что у меня заголовок с прозрачными областями... Но тут уж ничего не попишешь.
       
       А HTML выглядит достаточно прилично: &lt;h1&gt;&lt;span&gt;title&lt;/span&gt;&lt;/h1&gt;

     email: "plumbum@rambler.ru"

  -  author: "akella"
     id: "4379"
     url: "http://cssing.org.ua"
     date: "2006-08-15 20:11:13"
     humandate: "15 Aug, 2006"
     content: | 
       Самое прямолинейное решение с помощью javascript - http://www.whaleofadive.com/misc/siir/about.php - вообще же логичнее тогда оставить картинки :). Или сделать это на уровне сервера.

     email: "akella.a@gmail.com"

  -  author: "Dcat"
     id: "4371"
     url: "http://uaport.net"
     date: "2006-08-15 15:34:28"
     humandate: "15 Aug, 2006"
     content: | 
       А какие есть варианты для замены INLINE элемента на картинку?
       Например <b>:)</b> на картинку.

     email: "alex@visti.net"

  -  author: "akella"
     id: "4445"
     url: "http://cssing.org.ua"
     date: "2006-08-18 12:36:49"
     humandate: "18 Aug, 2006"
     content: | 
       Это для того что бы текст отобразился за пределами страницы, просто большое число что бы сдвинуть его(текст) из пределов видимости то бишь экрана. И что бы он не отображался поверх нашей картинки или чего либо еще на странице.

     email: "akella.a@gmail.com"

  -  author: "akella"
     id: "4474"
     url: "http://cssing.org.ua"
     date: "2006-08-19 09:18:00"
     humandate: "19 Aug, 2006"
     content: | 
       Такой метод(-1000em) считается более безопасным - и читатели экрана прочитают текст в первом случае - во втором могут и не прочесть.

     email: "akella.a@gmail.com"

  -  author: "Купер"
     id: "4454"
     url: "http://www.ipetra.ru/"
     date: "2006-08-18 18:25:33"
     humandate: "18 Aug, 2006"
     content: | 
       Так может просто в (или в css) сделать?

     email: "info@ipetra.ru"

  -  author: "Купер"
     id: "4455"
     url: "http://www.ipetra.ru/"
     date: "2006-08-18 18:26:09"
     humandate: "18 Aug, 2006"
     content: | 
       блин - я написал div style="display:none" в кавычках, а его "съело"

     email: "info@ipetra.ru"

  -  author: "Купер"
     id: "4442"
     url: "http://www.ipetra.ru/"
     date: "2006-08-18 12:17:41"
     humandate: "18 Aug, 2006"
     content: | 
       Не понял изврат с -1000em

     email: "info@ipetra.ru"

  -  author: "аниме"
     id: "10877"
     url: "http://www.fludilka.ru/"
     date: "2007-04-04 12:48:43"
     humandate: "04 Apr, 2007"
     content: | 
       есть один масюсенький минус, если такой фигни понаделать на сайте многократно, то не удивляйтесь, ежели у вас упадёт посещяемость!!
       
       Как говорится всё должно быть в меру!
       я прото, что, чтобы под картинкой ебыл спрятан роман война и мир!

     email: "kir_pich@yahoo.com"

  -  author: "Grin"
     id: "10990"
     url: "http://markovnin.com/"
     date: "2007-06-21 16:37:32"
     humandate: "21 Jun, 2007"
     content: | 
       хорошая статья, спасибо

     email: "pavel@markovnin.com"

  -  author: "Михаил"
     id: "11259"
     url: "http://turenko.com/blog/"
     date: "2007-11-01 07:53:34"
     humandate: "01 Nov, 2007"
     content: | 
       Скрытый текст по идее нехорошо, с точки зрения гугла...

     email: "mikhail@turenko.net"

  -  author: "Скакунов Александр"
     id: "11260"
     url: "http://i1t2b3.blogspot.com/"
     date: "2007-11-02 12:50:37"
     humandate: "02 Nov, 2007"
     content: | 
       Как называется классный шрифт, использованный на картинках в <a href="http://cssing.org.ua/examples/ir/" rel="nofollow">примерах<a>?

     email: "i1t2b3@gmail.com"

  -  author: "akella"
     id: "11262"
     url: "http://cssing.org.ua"
     date: "2007-11-02 14:13:27"
     humandate: "02 Nov, 2007"
     content: | 
       Вряд ли я смогу восстановить :( - но разве это не Scriptina? Я вроде бы не использовал чего то очень необычного

     email: "akella.a@gmail.com"

  -  author: "Скакунов Александр"
     id: "11263"
     url: "http://i1t2b3.blogspot.com/"
     date: "2007-11-02 16:33:04"
     humandate: "02 Nov, 2007"
     content: | 
       Вроде бы нет, но очень похоже, спасибо! 
       
       P.S. Было бы здорово иметь нотификацию по емейлу о приходящих комментариях, а то приходится по 20 раз открывать страницу, чтобы посмотреть глазами, ответил кто или нет.

     email: "i1t2b3@gmail.com"

  -  author: "akella"
     id: "11265"
     url: "http://cssing.org.ua"
     date: "2007-11-03 00:21:22"
     humandate: "03 Nov, 2007"
     content: | 
       Я надеялся что RSS достаточно, но добавил и форму подписки, спасибо за идею.

     email: "akella.a@gmail.com"

  -  author: "ArtDesigner"
     id: "11618"
     url: "http://artdesigner.ru"
     date: "2008-01-09 01:26:29"
     humandate: "09 Jan, 2008"
     content: | 
       Может я что-то где-то упустил, но я пользуюсь методом, который лишен недостатков. Возможно я не прав.
       h1 img src=”pic.png” alt=”Главная” /h1
       
       В браузерах отображается хорошо, с отключенными стилями картинки остаются, с отключенными картинками, альт заменяет сам заголовок. Когда всё отключено, также отображается верно. В чем подвох?

     email: "art@artdesigner.ru"

  -  author: "akella"
     id: "11625"
     url: "http://cssing.org.ua"
     date: "2008-01-09 13:09:10"
     humandate: "09 Jan, 2008"
     content: | 
       Ну некоторые оптимизаторы считают что альт меньше переливает в ссылку, или меньше веса придает словам, например. 
       А недостатков у метода действительно мало =) Разве что - чуть больше HTML, ведь нужно обязательно указать альт, адрес картинки, высоту и ширину.

     email: "akella.a@gmail.com"

  -  author: "Guyver"
     id: "11723"
     url: "http://guyver-world.ru/"
     date: "2008-01-24 01:25:55"
     humandate: "24 Jan, 2008"
     content: | 
       Хех, спасибо, буду пробовать на своих пациентах )

     email: "ilkart@rambler.ru"

  -  author: "Никита"
     id: "11905"
     url: "http://www.sexhtml.ru/"
     date: "2008-03-01 07:40:08"
     humandate: "01 Mar, 2008"
     content: | 
       <strong>h1{
        text-indent: -9000px;
       }</strong>
       
       Пользователи с отключенной графикой не увидят текст. Я использую похожую технику, только без смещения текста: http://www.sexhtml.ru/css/menu/

     email: "nikita.mosiyash@gmail.com"

  -  author: "Перспективный блоггер"
     id: "14445"
     url: "http://blogto4ka.ru"
     date: "2009-05-14 10:34:52"
     humandate: "14 May, 2009"
     content: | 
       Смотрю в ff3, в методе Маларки наблюдаю на картинке первую букву текста - "З", что вполне естественно, т.к. отрицательный letter-spacing не изменяет позицию первой буквы.
       
       Здесь нужно бы еще отрицательный text-indent на ширину первой буквы добавить, но тогда это уже будет метод, объединенный с методом Фарка.

     email: "Nikolas_Sharp@bigmir.net"

  -  author: "Del'ka"
     id: "12956"
     url: "http://delka.anime.kharkov.ua"
     date: "2008-07-24 13:49:58"
     humandate: "24 Jul, 2008"
     content: | 
       сегодня нашёл совершненно замечательный способ через :after
       http://habrahabr.ru/blog/css/37811.html
       
       хорош тем чо при отключенных картинках виден текст, но при этом нет несемантических span.

     email: "delka@anime.kharkov.ua"

  -  author: "cssing :: Архив :: Оценка качества верстки"
     id: "13354"
     url: "http://cssing.org.ua/2007/10/24/html-quality/"
     date: "2008-10-04 09:58:25"
     humandate: "04 Oct, 2008"
     content: | 
       [...] Последний хоткей кстати проявляет &#8220;плохие&#8221; image replacement [...]

     email: ""

  -  author: "Вредная верстка | Server Room"
     id: "37834"
     url: "http://it-hfs.ru/?p=94"
     date: "2012-01-26 18:22:43"
     humandate: "26 Jan, 2012"
     content: | 
       [...] Но как?! Читаем про LIR и Pixy. [...]

     email: ""

  -  author: "Вредная верстка &#8212; m1r8"
     id: "419158"
     url: "http://m1r8.ml/vrednaya-verstka/"
     date: "2017-04-07 05:59:26"
     humandate: "07 Apr, 2017"
     content: | 
       [&#8230;] Читаем про LIR и Pixy. [&#8230;]

     email: ""

layout: "layouts/post.njk"
excerpt: "Обзор некоторых способов замены текста картинками."
---

Обзор некоторых способов замены текста картинками.<!--more-->
<h3>Зачем?</h3>
Часто хочется чтобы заголовки были красивыми, и не хочется себя ограничивать парой тройкой шрифтов пользователя (из тех что есть у всех) &#8212; тут и приходят на помощь способы заменить этот текст (оставить его в коде для поисковиков и других юзер агентов) на картинки или флэш. Итак для начала заменяем такой код на картинку:
<ol class="code">
<li>&lt;h1&gt;Заголовок - картинка&lt;/h1&gt;</li>
</ol>
<h3>1. Способы без добавления HTML</h3>
Именно их я, как правило, и использую, если не нужно сильно заморачиваться на поддержке браузерами. Самые популярные:
<strong>1.</strong> LIR (<a href="http://www.moronicbajebus.com/playground/cssplay/image-replacement/">пример </a>) (так же известен как Phark Method)
<ol class="code">
<li>h1{</li>
<li class="tab">text-indent: -9000px;</li>
<li class="tab">overflow: hidden;</li>
<li class="tab">height:80px;width:200px;</li>
<li class="tab">background-image: url("img.gif");</li>
<li>}</li>
</ol>
Этот первый я чаще всего и применяю. Хотя при отключенных картинках мы не увидим ничего :(. Руководствуюсь принципом: &laquo;нефиг&raquo;. :)

<strong>2.</strong> Метод Leahy/Langridge  (<a href="http://www.kryogenix.org/code/browser/lir/">подробнее</a>)
<ol class="code">
<li>h1{</li>
<li class="tab">padding: 80px 0 0 0;</li>
<li class="tab">overflow: hidden;</li>
<li class="tab">background-image: url("img.gif"); </li>
<li class="tab">height: 0px !important; <small>/* для большинства броузеров */</small></li>
<li class="tab">height /**/:80px; <small>/* для блочной модели IE5.5 */</small></li>
<li>}</li>
</ol>
Вместо 80px естественно нужно вставить свою высоту.

<strong>3.</strong> MIR (Malarkey Image Replacement)  (<a href="http://www.stuffandnonsense.co.uk/archives/mir_image_replacement.html">подробнее</a>)
<ol class="code">
<li>h1{</li>
<li class="tab">letter-spacing :-1000em;</li>
<li class="tab">height:80px;width:200px;</li>
<li class="tab">background-image: url("img.gif");</li>
<li>}</li>
</ol>
Довольно изящный метод.
Все три разумеется при отключенных картинках не покажут ничего. Следует это помнить. Доступность страдает, но иногда бывают ситуации в которых эти методы могут сильно выручить. <a href="http://cssing.org.ua/examples/ir/">Смотреть пример.</a>
<h3>2. Способы c добавлением HTML</h3>
<strong>1.</strong> Метод  Pixy  (<a href="http://wellstyled.com/css-replace-text-by-image.html">подробнее</a>)
<strong>HTML:</strong>
<ol class="code">
<li>&lt;h1&gt;Заголовок - картинка&lt;span&gt;&lt;/span&gt;&lt;/h1&gt;</li>
</ol>
<strong>CSS:</strong>
<ol class="code">
<li>h1{</li>
<li class="tab">margin:0; padding:0;</li>
<li class="tab">position:relative;</li>
<li class="tab">width:200px; height:80px;</li>
<li class="tab">overflow:hidden;</li>
<li>}</li>
<li>h1 span {</li>
<li class="tab">display:block;</li>
<li class="tab">position:absolute; left:0; top:0; z-index:1;</li>
<li class="tab">width:200px; height:80px;</li>
<li class="tab">background:url("img.gif") top left no-repeat;</li>
<li class="tab">}</li>
</ol>
Если картинки отключены текст будет видно. Один из лучших методов, главное не забыть вставить спан. По сути фоновая картинка ложится сверху на текст и при ее отсутствии текст просвечивает.
Есть еще несколько вариаций которые работают в тех же браузерах (ИЕ 5 и выше и все остальные более или менее новые) но отличаются немного структурой кода:  <a href="http://levin.grundeis.net/files/20030809/alternatefir.html">Levin Alexander's</a> например.
<strong>2.</strong> Thierry Image (re)Placement  (<a href="http://www.tjkdesign.com/articles/tip.asp">подробнее</a>)
<strong>HTML:</strong>
<ol class="code">
<li>&lt;h1&gt;&lt;img src="pic.gif"  /&gt;Заголовок - картинка&lt;/h1&gt;</li>
</ol>
<strong>CSS:</strong>
<ol class="code">
<li>h1 {</li>
<li class="tab">height:80px;</li>
<li class="tab">width:200px;</li>
<li class="tab">overflow:hidden;</li>
<li class="tab">position:relative;</li>
<li>}</li>
<li>h1 img {</li>
<li class="tab">z-index:1;</li>
<li class="tab">position:absolute;</li>
<li class="tab">top:0;</li>
<li class="tab">left:0;</li>
<li>}</li>
</ol>
<h3>Другие способы</h3>
Среди прочих нельзя не упомянуть <a href="http://www.mikeindustries.com/sifr/">sIFR</a> (и <a href="http://www.maratz.com/blog/archives/2006/01/16/multi-color-sifr-201/">неофициальные апгрейды</a> к нему) &#8212; замена с помощью флеша и джаваскрипта.
И некоторые методы замены картинками еще на сервере: <a href="http://www.alistapart.com/articles/dynatext">Dynamic Text Replacement</a> и на русском <a href="http://www.umade.ru/log/2006/01/167.html">PHP+CSS: Динамичеcкая замена текста</a>.
А так же то, к чему мы прийдем рано или поздно :), CSS3 метод замены текста:
<ol class="code">
<li>h1 {</li>
<li class="tab">content: url(img.gif);</li>
<li>}</li>
</ol>
Ну или простой и банальный font-face, который наконец заработает везде.
<h3>Ссылки</h3>
Собственно не такой же ж я умник что бы самому вот это все придумать. :)
К тому же это далеко не полный список методов, лишь те, которые я практикую и считаю удобными для себя. 
<ul>
<li><a href="http://cssing.org.ua/examples/ir/">Мои примеры - для теста</a></li>
<li><a href="http://www.mezzoblue.com/tests/revised-image-replacement/">Revised Image Replacement</a></li>
<li><a href="http://css-discuss.incutio.com/?page=ImageReplacement">CSS Image Replacement and Alternatives to CSS Image Replacement</a></li>
</ul>
Линков из этих двух страничек хватит всерьез и надолго :)
С названиями полная путаница, поэтому называл я по имени того кто выше в гугле. Хоть для какой то ориентации.
