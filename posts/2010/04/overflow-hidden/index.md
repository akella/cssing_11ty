---
title: "overflow:hidden"
date: "2010-04-26"
categories: 
  - "xhtmlcss"
---

Незаслуженно непопулярный трюк. Я уже писал про [display:table](http://cssing.org.ua/2005/07/03/display-table/). Так вот, это — лучше. P.S.: оказалось трюк таки известен многим, надеюсь кому-то статья поможет.

### Проблема

Еще пять лет назад я искал решение проблемы: как запретить обтекание float. Подробнее можно читать в [старом посте](http://cssing.org.ua/2005/07/03/display-table/) (2005 год, офигеть). Вкратце, мы приводили это:

![](http://cssing.org.ua/pic/overflow/1.png)Картинка-float

к такому виду:

![](http://cssing.org.ua/pic/overflow/2.png)Картинка-float + display:table для текста

Для этого тексту задавалось свойство display:table. А для IE zoom:1.

### overflow:hidden magic

Относительно недавно (относительно пяти лет) мы столкнулись с новым способом, оказалось что overflow:hidden может повторить этот эффект, и [сделать его даже лучше](http://cssing.org.ua/examples/overflow-hidden/). Причина обоих трюков, вовсе не глюки браузеров или специфика их отображения. Причина на сайте W3C:

> The border box of a table, a block-level replaced element, or an element in the normal flow that establishes a new block formatting context (such as an element with ‘overflow’ other than ‘visible’) must not overlap any floats in the same block formatting context as the element itself. W3C, CSS 2.1

[источник](http://www.w3.org/TR/CSS2/visuren.html#floats) То есть это не хак, а документированное поведение. Всё дело в так называемом «контексте» или «контексте форматирования», такие правила как display и overflow создают этот контекст, и согласно правилам он (созданный контекст) не может пересекаться с флоатами. Что вобщем и происходит. В результате блок занимает все доступное пространство _кроме флоата_.

> Floats, absolutely positioned elements, inline-blocks, table-cells, table-captions, and elements with 'overflow' other than 'visible' (except when that value has been propagated to the viewport) establish new block formatting contexts.

Как видим контекст можно создавать разными способами.

Важное отличие от display:table — _ширина блока_, я сделал [специальный пример](http://cssing.org.ua/examples/overflow-hidden/index_text.html) чтобы было видно, чем часто был неудобен именно display:table.

Именно это отличие позволяет делать с overflow более сложные вещи чем с display:table.

![](http://cssing.org.ua/pic/overflow/tablehidden.png)Когда мало текста, блок не занимает всю ширину

### IE?

**IE6** — не работает ни display:table ни overflow:hidden. Нужно использовать zoom:1; (или любой hasLayout). В результате эффект идентичен действию overflow в других браузерах.

**IE7-8** — overflow:hidden работает также как во всех остальных возможных браузерах.

Резюмируя: можно добавить к overflow:hidden еще zoom:1; и забыть о проблеме.

### Возможные применения

Самое простое и банальное, вёрстка [блоков с текстом и картинкой](http://cssing.org.ua/examples/overflow-hidden/index_pic.html):

![](http://cssing.org.ua/pic/overflow/2.png)Редкий сайт обходится без такого блока

Используя overflow:hidden можно их стилизовать для произвольной ширины картинок.

Чуть более сложный кейс, [резиновый инпут и кнопка](http://cssing.org.ua/examples/overflow-hidden/index_input.html):

[![](http://cssing.org.ua/pic/overflow/input.png)Обычное дело на резиновых сайтах](http://cssing.org.ua/examples/overflow-hidden/)

С подобной проблемой недавно столкнулся Глеб Арестов и [успешно решил](http://friendfeed.com/yodapunk/c1ada988) её как раз с помощью этого же свойства.

Более того, можно строить layout страниц. В частности в фреймворке [OOCSS](http://wiki.github.com/stubbornella/oocss/) колонки строятся как раз с использованием этого свойства. Примерно так:

[![](http://cssing.org.ua/pic/overflow/layout.png)Можно не задавать ширину резиновой колонке](http://cssing.org.ua/examples/overflow-hidden/index_layout.html)

Конечно, тут минимум два недостатка. Во-первых, порядок контента — средняя колонка должна идти в коде после обоих боковых. Во-вторых, нестабильность при сжатии, когда что-то начинает не помещаться в блоке с overflow:hidden, его самым невероятным образом разрывает на части в IE. min-width мог бы спасти. [Использовать](http://cssing.org.ua/examples/overflow-hidden/index_layout.html) осторожно.

Но, помнить о таком мощном приеме стоит.

### Еще

- [Пост Gunlaug](http://www.gunlaug.no/contents/wd_example_01_01.html) про это же поведение
- [Мой пост про display:table](http://cssing.org.ua/2005/07/03/display-table/)
- [Мой простой пример](http://cssing.org.ua/examples/overflow-hidden/), [пример трехколоночного сайта](http://cssing.org.ua/examples/overflow-hidden/index_layout.html)
- [Пост Flack на эту же тему](http://flack.ru/2008/08/26/semantic-coding-howto-6/)
- [Clear или overflow:hidden — очистка всего потока или создание контекста форматирования?](http://habrahabr.ru/blogs/css/48383/)
- [Управление потоком в CSS: создаём контекст форматирования](http://habrahabr.ru/blogs/css/48429/)

Это не CSS3 и далеко не вчерашнее изобретение, но кажется многие недооценивают силу этого простого приема.

Буду рад если поделитесь своим опытом!
