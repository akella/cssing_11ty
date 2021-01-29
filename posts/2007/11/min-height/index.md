---
title: "Cколько-то способов min-height"
date: "2007-11-29"
categories: 
  - "xhtmlcss"
  - "useful"
---

Несколько способов реализации min-height для всех броузеров. Короткий обобщающий пост. Надеюсь все оценили как я изящно избежал цифры в названии поста?=) Свойство нужное, часто полезное, но в Internet Explorer не работает. Далее способы вразумить синюю букву Е.

### 1\. min-height через height

Говорят, разработчики IE5-6 **реализовали** свойство min-height, просто решили его назвать height, так оно вобщем то и есть. height для 5й и 6й версий ведет себя как min-height. В 7й версии min-height уже работает. Потому вопрос лишь в том, как им всем отдать свои значения. Об этом позаботился Дастин Диаз:

1. .block {
2. min-height:200px;
3. height:auto !important;
4. height:200px;
5. }

Комментировать особо нечего - это работает. Первая колонка в [примере](http://cssing.org.ua/examples/min-height/).

На данный момент, в силу того что ИЕ7 уже поддерживает min-height, два другие способа я привожу скорее как историческую справку и пример интересных приемов.

- [оригинальная статья](http://www.dustindiaz.com/min-height-fast-hack/)

### 2\. min-height с помощью padding

Так же можно эмулировать минимальную высоту с помощью комбинации:

1. .block{padding-top:200px}
2. .block .inner{margin-top:-200px}

Этот способ требует однако дополнительного элемента ".inner", тем не менее является пожалуй самым простым и иногда удобным. Что бы кусок кода был максимально универсальным - лучше добавлять аж 2 обертки:

1. .block .inner{padding-top:200px}
2. .block .inner1{margin-top:-200px}

В [примере](http://cssing.org.ua/examples/min-height/) я вместо второй обертки использовал элемент h2.

- Подробнее в блоге [у Dave Shea](http://www.mezzoblue.com/archives/2004/09/16/minheight_fi/)

### 3\. min-height с помощью expression

Как всегда все можно решить с помощью джаваскрипт.

До того как вышла 7ая версия можно было делать так:

1. .block{height: expression('32px'); min-height: 32px;}

Однако этот вариант не работает в 7й версии.

Более универсально и в лоб, проблема решается так:

1. .block {
2. height: expression(this.scrollHeight < 201px ? "200px" : "auto" );
3. min-height: 200px;
4. }

Или что бы ускорить работу скрипта, как [советует](http://cssing.org.ua/2007/11/29/min-height/#comment-11392) [Павел Корнилов](http://lusever.ru), `this` можно опустить:

1. .block {
2. height: expression(scrollHeight < 201px ? "200px" : "auto" );

Для body, однако, так нельзя оптимизировать.

### В конце

- [Пример с тремя методами](http://cssing.org.ua/examples/min-height/)

Буду рад услышать ваши методы и мысли по поводу решения этой проблемы!