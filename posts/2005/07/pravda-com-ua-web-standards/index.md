---
title: "pravda.com.ua!"
date: "2005-07-23"
categories: 
  - "web-standards"
---

Сегодня еще один посещаемый украинский сайт (а именно [3ий](http://top.bigmir.net/show.php?u=1) в Украине) и [самый](http://top.bigmir.net/show.php?ctg=39&u=1&t=0) популярный новостной ресурс - [Украинская Правда](http://pravda.com.ua/) перешел на вебстандарты.

### Бочка меда

Привожу небольшие замеры выгоды для юзеров:

|   | Старый код | Новый код |
| --- | --- | --- |
| Размер CSS файла | ~6 KB | ~12 KB |
| Размер HTML файла | ~106 KB | ~45 KB |
| Общая Экономия(На HTML) | \- | **~60Kb** |

За понимание и содействие хочу сказать огроменное СПАСИБО **Алене Притуле**(главред) и **Tadjik**'у(webmaster)!

В килобайтах разница еще круче чем с [Укр.Нет](http://cssing.iatp.org.ua/2005/02/16/ukrnet/). Дизайн опять же(как и с Укр.Нет) был повторен, что вызвало появление пары "лишних" DIV для копирования table-like эффектов.

К тому же теперь любую страницу этого сайта можно рачпечатывать (_media="print"_). А для мобильных девайсов я отключил графику - дабы экономить траффик (_media="handheld"_), хотя это конечно спорное решение. И добавил SKIP-menu - для навигации по длинным страницам. Изначально дизайн был с фиксированными размерами шрифтов - поэтому я не косил под "настоящего" вебстандартиста и в вебстандартной версии размеры указывал в пикселах. Но я вынес их(все font-size) в [отдельный файл](http://pravda.com.ua/_site/css/MainSm.css) и добавил [styleswitcher](http://www.alistapart.com/articles/alternate/). Правда позднее было решено оставить его лишь на странице с полным текстом статей, но сугубо из "дизайнерских" соображений - некуда впихнуть. :)

Так что за пикселы чур не казнить! :)

### Ложка дегтя

К сожалению есть ряд проблем которые я не в силах был решить. Например все старые статьи останутся в виде

Abzac
**<br><br>**
Abzac

И еще кучей фигового кода - который однако умудряется работать правильно в окружении нормального кода.

Более того "порадовала" CMS, редактор статей которой генерит все тэги большими буквами, а иногда при вставке картинки - выдаёт такие перлы из набора DIV и TABLE - что хоть стой хоть падай. Так что вебстандартами это пока можно назвать все же с натяжкой(но бои с CMS продолжаются.) - из-за текста самих статей. :(

Хотя ИМХО шаг мы сделали в правильном направлении.

Ни о какой валидности пока не может быть и речи - при нашей баннерной системе и куче невалидных каунтеров - привести сайт к абсолютно валидному коду - самоубийство. Но не стоит забывать что валидация нужна прежде всего нам - разработчикам. Не закрой я там какой нить один ДИВ - была бы страшная картина...

### Feedback

Был бы очень рад услышать Ваше мнение по поводу кода. Я понимаю что я несовершенен и какой то глюк мог и упустить при переходе на новый код. Поэтому комменты типа "а че оно все сползло вниз" с радостью принимаются, но при указании броузера и системы. **Заранее спасибо!**

PS: скоро опишу некоторые полезности разработки кода для подобных сайтов..

### Предмет критики

- [Украинская правда](http://pravda.com.ua/)
- Один из [последних моих темплейтов](http://akella.org.ua/pro/pravda.com.ua/) перед началом реализации