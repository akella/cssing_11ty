---
title: "Микроформаты в жизнь!"
date: "2007-12-21"
categories: 
  - "xhtmlcss"
  - "thoughts"
  - "common"
---

Мои(и не только) мысли о микроформатах. А так же нескольно примеров проектов, в которых я применял микроформаты.

### Что это

Всего лишь предопределенные имена классов, и тагов. Не более того. Смотрите сами, ХТМЛ до микроформатов:

1. <dd>
2. Юрий Артюх,
3. +38 096 970-6428,
4. <a href="mailto:...">akella.a@mail.com</a>
5. </dd>

И после:

1. <dd class="vcard">
2. <span class="fn">Юрий Артюх</span>,
3. <span class="tel">+38 096 970-6428</span>,
4. <a class="email" href="mailto:...">akella.a@mail.com</a>
5. </dd>

Добавилися класс показывающий тип формата — vcard. Спаны, для того чтобы "машины" разобрались где телефон, имя и адрес. Вот и все. Делов то. Зато какие перспективы!

### Зачем это

Представьте себе 1970 год. Вся информация об организациях хранится в бумажном каталоге, "Желтые страницы" например. Обновляется раз в год, а то и реже. А потом еще полгода чтобы издать.

Далее, 2000й год, уже есть сайт, на который сотни модераторов, или фирмы сами, добавляют данные о себе. После чего пользователь может на сайте получить всё ту же информацию, что из желтых страниц. Которая, однако редко обновляется. Попробуй уследи за адресами сотни тысяч фирм..

А теперь представьте, год 2010й. Каждая фирма обновляет свою информацию у себя на сайте. Где она разметила ее в hcard. Таким образом, при наличии поисковика по формату, мы будем иметь всё те же "Желтые страницы", но **обновляющиеся моментально**. (я принимаю интернетизацию общества за данность). Фирмам не нужно нигде регистрироваться, просто обновить инфо на своем сайте!

По сути это шаг от централизованных систем к распределенным. Тот же веб2.0 в некотором смысле шагнул, от централизованной генерации контента, к распределенной. И этот тренд видно практически во всех областях. Это наводит на мысли о правильности пути микроформатов.

В примере выше я упоминал формат hcard, но попробуйте представить распределенную систему оценок для фильма, или подписку прямо на страничке с форматом hAtom, без поиска RSS-каналов. Или обновление своей адресной книги, или то чудесное применение, что [придумал Иван Сагалаев](http://softwaremaniacs.org/blog/2007/03/25/cicero-openid-hcard/).

Примерно так бы я распределил сервисы и их аналоги по сущностям в микроформатах (на самом деле, мне просто нравится новый дизайн таблиц на блоге):

|   | Цетрализованная система | Распределённая |
| --- | --- | --- |
| Новости | Feedburner, news.google.com | hAtom |
| Адресная книга | plaxo, linkedin, facebook (vkontakte) | hCard + XFN |
| Календари | upcoming, ckopo.in.ua | hCalendar |

### Микроформаты и Wordpress

Как пример микроформатизации можно рассмотреть Wordpress, хотя практически все новые темы выходят с учетом hAtom. Тем не менее, сейчас у меня вот такой кусочек кода в /wp-content/wp-themes/wpthemename/index.php выводит список заметок:

1. <div class="hentry">
2. <h2 class="entry-title"><a href="<?php the\_permalink() ?>" rel="bookmark" title="пермалинк <?php the\_title(); ?>">...</a></h2>
3. <abbr class="published" title="<?php the\_time('Y-m-d\\TH:i:sO'); ?>"><?php the\_time('j F, Y') ?></abbr>
4. <div class="entry-summary"><?php the\_content('читать дальше'); ?></div>
5. </div>

Результатом будет такой HTML, я выделил жирным все, что добавлено для микроформатов:

1. <div class="hentry">
2. <h2 **class="entry-title"**\><a href="#" **rel="bookmark"**\> ... </a></h2>
3. <abbr **class="published"** title="**2007-12-06T16:36:10+0200**">6 октября, 2007</abbr>
4. <div **class="entry-summary"**\>Выдержка из поста</div>
5. </div>

Как видно, всего лишь классы. Для даты принят стандартный формат **<abbr title="2007-12-06T16:36:10+0200"**, вдобавок вся новостная лента должна быть обернута в див с классом `hfeed`.

- [Спецификация hAtom (draft)](http://microformats.org/wiki/hatom)
- [Спецификация hcard](http://microformats.org/wiki/hcard)

### XFN

Так называется формат нагружающий смыслом ссылки. XFN — XHTML Friends Network. Здесь вообще все элементарно, вот одна из ссылок в правой колонке моего блога:

1. <a href='http://uggallery.audiopeace.ru/' rel='**acquaintance met colleague**'>Александр Исаков</a>

Что означает, что я знаком с этим человеком(acquaintance), встречал его вживую(met) и являюсь его коллегой(colleague). Подробнее можно почитать на [главной странице XFN](http://gmpg.org/xfn/)

### В конце

Несмотря на то, что идее уже третий год, и даже Билл Гейтс считает ее удачной, она(идея) все еще в развивающемся состоянии. И думаю во многом это зависит от разработчиков. Изучение микроформатов все же является неким риском. Никто не гарантирует во что это все выльется. Тем не менее, я их использую в большинстве своих проектов уже сейчас. Потому что это просто.

- [microformats.org](http://microformats.org/) — главный ресурс где и находится [wiki c полным описанием](http://microformats.org/wiki/) и возможностью проапдейтить формат или задать вопрос
- [Этому сервису](http://microformatique.com/optimus/) можно скормить УРЛ странички, он же выделит на ней все известные микроформаты, [вот так например](http://microformatique.com/optimus/?uri=http://cssing.org.ua), к сожалению пока там легки проблемы с кириллицей =(. Но автор проекта Дмитрий Барановский уверен это поправит.
- [Официальная страничка плагина Tails для Firefox](http://blog.codeeg.com/tails-firefox-extension-03/) и [плагин для экспорта микроформатов](https://addons.mozilla.org/en-US/firefox/addon/2240) в другие приложения
- [Микроформаты убьют Facebook](http://lucidplot.com/2007/07/12/microformats-kill-facebook/)

Ваши мысли о перспективах микроформатов приветствуются!