---
title: "HTML заготовки"
date: "2005-08-24"
categories: 
  - "xhtmlcss"
  - "useful"
---

На горизонте, как тучи, собирается работа... Решил не ждать - а начать готовиться. Подготовил серию XHTML заготовок.

### Зачем?

Каждый раз когда я начинаю верстать, я заново ворую где то доктайп, создаю CSS файлы - переписываю метатэги с какого-нить доверенного сайта. Но, наконец, чаша полна. Лень ослабла, и я решился сделать стартовые HTML+CSS заготовки. Кому сгодятся - используйте на здоровье...

### HTML

Не буду тут приводить полностью файл. Однако я в него насовал все метатэги которые я использовал. Вот небольшой такой список:

1. <meta http-equiv="Content-Type" content="text/html; charset=windows-1251" />

3. <meta http-equiv="Content-Language" content="ru" />
4. <meta name="copyright" content="" />
5. <meta name="description" content="" />
6. <meta name="keywords" content="" />
7. <meta name="author" content="" />
8. <meta name="robots" content="all" />
9. <link rel="Shortcut Icon" type="image/x-icon" href="/favicon.ico" />

Я выбирал самое нужное для себя - если у кого есть чем дополнить - пожалуйста в комменты...

Плюс ссылки на (смотри ниже) CSS файлы

### CSS

Главная страница ссылается на 3 CSS файла: **master.css print.css handheld.css**. Которые все лежат в папке **css**.

Содержание master.css примерно такое:

1. @import url("base.css");
2. @import url("layout.css");

И еще сколько влезет разделений на стили для **цвета**, **шрифтов**. Просто я использую пока именно такое разделение.

Все CSS файлы снабжены заботливо спертыми заголовками у Дага Баумана (нравятся они мне :)) Вот такого вида:

1. /\*
2. \-----------------------------------------------
3. Site Screen Master
4. Author: akella
5. Version: 28 Apr 1983
6. \----------------------------------------------- \*/

### Результат

В результате вышло такое: ![file tree of template](http://cssing.org.ua/images/tree.png) Скачать все сразу можно [отсюда](http://cssing.org.ua/examples/template/template.rar). Посмотреть вживую - [тут](http://cssing.org.ua/examples/template/). (нажимайте вью сорс) Для маленьких сайтов(воробьев) - это конечно скорее пушка, но для средних проектов самое то. Да и пушкой в принципе убить воробья - не так и трудно :).

### Инфо

- [Architecting CSS](http://www.digital-web.com/articles/architecting_css/)
- [XHTML templates](http://particletree.com/features/quick-start-your-design-with-xhtml-templates)

Замечания-указания-поправки с радостью принимаются )
