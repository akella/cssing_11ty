---
title: "Поиск Данстана"
date: "2004-12-06"
categories: 
  - "xhtmlcss"
  - "useful"
---

Немного оклемался от революции и на глаза попалась классная штука. Еще одну великолепную идею подарил нам [Данстан Орчард](http://www.1976design.com/blog/)([уточнение](#update)). Если вы еще не знаете попробуйте поискать на его сайте чего-нибудь.(Enter не нажимать!) Вот решил разобраться как же такое делать. Вдруг еще кому окажется полезным.

### В чем фишка?

Главная фишка этого "живого" поиска в том, что страница не обновляется, когда вы ищете что-нибудь. Как это возможно?

### XML HTTP Request

Не буду излагать всю статью. Главное, что этот объект позволяет javascript делать HTTP запросы и получать на них ответ. Это открывает немерено возможностей. И одно из самых главных - мы можем обновлять некоторую информацию на странице **без** ее(страницы) обновления полностью. Подробнее об использовании этого объекта читайте здесь: [Using the XML HTTP Request object](http://jibbering.com/2002/4/httprequest.html) (там есть некоторые оговорки с поддержкой, но Мозилла и ИЕ работают)

### Не только javascript

Однако одним джаваскриптом тут не обошлось. Ведь надо получить из базы результаты поиска. Поэтому скрипт вызывает php файл поиска и оттуда черпает результаты.

### Все вместе

В целом если опустить мелочи касательно задержек, очистки поиска и тому подобного. То можно так представить этот поиск:

1. Создается объект и примерно такой строкой запрашиваем результат поиска:
    
    liveSearchReq.open('GET', processURI+searchInput.value);
    
    При этом нам надо использовать специальный скрипт для поиска. Он должен возвращать **не целую страницу**, а лишь тот **кусок HTML кода**, который мы хотим отобразить сразу. То есть лишь результаты поиска.(без тэгов BODY, HTML)
2. С помощью DOM создаем `DIV` в который и пишем эти результаты.
3. Любуемся "живым" поиском

### Наконец

Блог Данстана это просто кладовая замечательных скриптов. Я наверно не раз еще вернусь и почерпну что-нибудь полезное оттуда.

### Проблема

Почему то появились глюки с кодировкой. Как я ни гадал ЮТФ и Вин-1251 не подходят. Причем ИЕ кодировку почему то угадывает. А как бороться в других случаях, я так и не смог понять. Быть может кто-то сталкивался с подобным? Откликнитесь в комменты.

Можно посмотреть на поиск на сайте Данстана, но это неинтересно (там не глючит кодировка :) ) Поэтому вот здесь я привожу вариант с глючной кодировкой. [Мой вариант "живого" поиска.](http://cssing.iatp.org.ua/antry.php). Не все там гладко и со стороны Wordpress'a, когда результат поиска одна заметка этот гад (:)) делает переадресацию и выводит и HTML и BODY тэг. Но это не проблема. А вот кодировка...

### Уточнение

**Восстанавливая справедливость.** Авторство данной техники принадлежит Christian Stocker. И подробнее о ней можно прочитать здесь [http://blog4.bitflux.ch/wiki/LiveSearch](http://blog4.bitflux.ch/wiki/LiveSearch "LiveSearch")