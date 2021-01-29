---
title: "G-club, микроформаты и дизайн"
date: "2008-08-08"
categories: 
  - "tusovka"
---

Выступали в [g-club](http://www.globallogic.com.ua/globallogic/index.php?option=com_content&task=view&id=17213&Itemid=124), замечательной инициативе от компании [GlobalLogic](http://www.globallogic.com.ua/globallogic/). Я рассказывал о вёрстке и микроформатах, [Гена](http://mega.genn.org/) забавно и увлекательно о том [как делать сайты](http://mega.genn.org/2008/08/07/sites-in-g-club/).

### Презентация

В ней куча скриншотов и картинок, основную часть информации я проговорил. 

### Краткое вступление

Кроме рассказа о компаниях и проектах с кодом которых я сталкивался или работал, я рассказал о том, что такое микроформаты, на паре простых примеров показал, _как легко их внедрять_. Затем рассказал о гугловском API для парсинга XFN связей. Вот несколько ссылок:

- [Микроформаты в жизнь](http://cssing.org.ua/2007/12/21/gogo-mf/) — мой старый пост о микроформатах
- [microformats.org](http://microformats.org/) — официальный сайт микроформатов
- [Google Social Graph API](http://code.google.com/apis/socialgraph/), тот самый интерфейс гугла, для получения XFN связей. [На примере CSSing](http://socialgraph-resources.googlecode.com/svn/trunk/samples/findcontacts.html?q=cssing.org.ua%0D%0A%0D%0A)
- [Portable Social Networks, The Building Blocks Of A Social Web](http://www.digital-web.com/articles/portable_social_networks_building_blocks_of_a_social_web/) — хорошая статья про социальные сети и XFN
- [Fundamentos Web: Social Network Portability](http://tantek.com/presentations/2007/10/social-network-portability/) — презентация Тантека Челика.

### Микроформаты для экономии времени

Проект toluu.com использует микроформаты для заполнения регистрационной инфо. Просто вводите ваш логин с Flickr, Upcoming или Twitter. Информация о вас будет взята оттуда: аватар, имя, сайт.

Убедиться можно на [этой страничке](http://www.toluu.com/join) (обратите внимание на блок «Use any of these?» справа).

### Yahoo & μF

Яху _уже_ может искать по микроформатам, и это замечательно. Запрос нужно отправлять вида:

searchmonkeyid:com.yahoo.uf.hcard YourKeyword

Для поиска по hCard. Ну и соответственно, поиск по hReview:

searchmonkeyid:com.yahoo.uf.hreview YourKeyword

На всякий случай, uf — одно из общепринятых сокращений слова микроформаты (u напоминает μ) Вот несколько готовых интересных ссылок (скрины в презентации):

- [Поиск всех hCard людей, где упоминается фамилия Artyukh](http://search.yahoo.com/search;_ylt=A0geu_GYAphI7xgBOjRXNyoA?p=searchmonkeyid%3Acom.yahoo.uf.hcard+artyukh&y=Search&fr=&ei=UTF-8), попробуйте со своим ником-именем-фамилией
- [Поиск всех hCard](http://search.yahoo.com/search;_ylt=A0geu_ES3ZpIgRIBf9hXNyoA?p=searchmonkeyid%3Acom.yahoo.uf.hcard&y=Search&fr=&ei=UTF-8), видно, что проиндексировано уже более миллиарда hCard
- [Поиск всех hReview о фотоаппарате Canon 400D](http://search.yahoo.com/search;_ylt=A0geu_GYAphI7xgBOjRXNyoA?p=searchmonkeyid%3Acom.yahoo.uf.hreview+400D&y=Search&fr=&ei=UTF-8), забавно что если бы было видно звездочки (оценки), можно бы было судить о фотоаппарате не кликая по ссылкам вообще
- [Поиск всех hReview о ресторанах со словом Higura](http://search.yahoo.com/search;_ylt=A0geu432oJlInhsAyCVXNyoA?p=searchmonkeyid%3Acom.yahoo.uf.hreview+higuma&y=Search&fr=&ei=UTF-8), а вот тут уже видно звездочки, здорово, да?

Для тех кто поленился кликать, вот картинка, значения для сереньких полей берутся из соответствующих полей в hCard (class="position" etc..):

![микроформаты на yahoo](http://cssing.org.ua/pic/mf.png)Микроформаты в действии!

(Синим отвратительным маркером я обозначил места на которые нужно обратить внимание.)

А это уже означает, что микроформаты дают преимущество в поиске. А значит помогают SEO, а значит... _приносят деньги_.

для такого отображения используется механизм SearchMonkey, который в свою очередь использует микроформаты. Но в моих мечтах яху начнет отображать их автоматически при заданном поиске по hCard или hReview

И ведь ничего не мешает yahoomen поставить вместо этого сложного запроса радиобуттон: «Искать в ревью» (hReview), «Искать в людях» (hCard), «Искать в событиях» (hCalendar).

Кажется, именно так они решили проблему [курицы и яйца](http://cssing.org.ua/2007/12/21/gogo-mf/#comment-11521). Как я уже говорил, поисковых механизмов по микроформатам нет, потому что недостаточно самих микроформатов в интернете. А микроформаты не внедряют на сайтах, потому что нет поиска по ним.

И вот, более миллиарда hCard и 46 миллионов hReview. And counting...

Подробнее о Searchmonkey (кастомизации результатов поиска) читайте в блоге талантливого разработчика Артемия Трегубенко «[микроформаты, yahoo, searchmonkey](http://blog.arty.name/2008/mikroformatyi-yahoo-searchmonkey/)». Там же, пример профиля сайта для mirtesen.ru.

### Фотки

![гена не упустил шанса что-то написать](http://cssing.org.ua/pic/gclub/1.jpg)Гена решил разрядить обстановку

![гена не упустил шанса что-то написать](http://cssing.org.ua/pic/gclub/2.jpg)Геннадий, какой-то парень, зал и сложный вопрос (слева направо)

За фото спасибо Константину Кудрявцеву! Жаль только не видно, что выступали мы с Macbook Air, iBook и iPhone =)

### В конце

- [Отчет Геннадия Осипенко](http://mega.genn.org/2008/08/07/sites-in-g-club/), там же его презентация с полным текстом доклада
- [Другие мероприятия в g-club](http://globallogic.com.ua/globallogic/?option=com_content&task=view&id=17640&Itemid=131)

Не то чтобы информация из доклада была сильно уникальна, но меня бы заели друзья за то, что я не пересказал свой доклад.

Получилось неплохо! Еще десяток выступлений и мои связки окончательно окрепнут. =)
