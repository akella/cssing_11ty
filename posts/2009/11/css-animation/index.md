---
title: "Всё крутится и летает"
date: "2009-11-04"
categories: 
  - "fun"
  - "xhtmlcss"
---

Я занимался сексом с webkit-transition, результат [можно увидеть тут](http://cssing.org.ua/examples/cssanimation/), да и [тут впрочем тоже](http://cssing.org.ua/examples/cssanimation/letters-comp-scaledelayrotate.html), а [вот что придумал Genn](http://genn.org/junk/kit3.html) узнав об этом (примеры работают пока только в Хроме и Сафари).

Дальше будет немного теории, можно сразу перейти к примерам внизу.

### transition transform

Это CSS3 свойства, которые пока работают только в Safari и Chrome. Еще они будут в следующей версии Firefox и Opera. Но пока нет.

Если вам совсем нечего делать, можно прочитать о них в [спецификации про 2d-transforms](http://www.w3.org/TR/css3-2d-transforms/) и [про transitions](http://www.w3.org/TR/css3-transitions/). Это всё конечно draft, но вряд ли что-то изменится.

Вкратце всё обстоит так.

**transform** — совершает всякие странные эффекты с блоком. По сути похоже на text-transform, просто эффекты более странные. Например можно писать так:

1. .weirdblock{
2. transform: rotate(45deg) scale(2);
3. }

Путем невероятных мыслительных усилий, вы уже могли бы догадаться что этот код повернет блок на 45 градусов, и увеличит его в размере в два раза, без анимации, просто такой моментальный эффект.

![](/pic/ex.png)Был маленький и прямой, стал большой и кривой

Пока спецификация неактуальна, для Сафари и Хрома правило нужно писать с префиксом `-webkit-`. То есть вот так:

1. .weirdblock{
2. \-webkit-transform: rotate(45deg) scale(2);
3. }

Вот вобщем и всё, transform уже работает в последнем Фаерфоксе, кстати. [Подробнее о нём](http://webkit.org/blog/130/css-transforms/).

**transition** — определяет анимацию блока. Используется примерно так:

1. div{
2. opacity:0.5;
3. \-webkit-transition: opacity 1s linear; /\*opacity - что анимируем,1s - длительность эффекта, linear - плавность эффекта\*/
4. }
5. div:hover{
6. opacity:1;
7. }

По наведению курсора, блок просто плавно изменит свою прозрачность за 1 секунду. Это мог бы быть фон, размер и цвет текста и все что угодно. [Всё можно анимировать](http://webkit.org/blog/138/css-animation/). А вот так например можно плавно менять цвет ссылки по наведению мыши:

1. a{
2. color:green;
3. \-webkit-transition:all 1s linear;
4. }
5. a:hover{
6. color:red;
7. }

А теперь примеры! ;)

### Примеры (пока только для Safari и Chrome)

Анимация во всех примерах начинается по наведению мышки. Когда убираете мышку, она проигрывается до исходного состояния.

Первое что пришло в голову, сделать анимированный комикс ;) [Вот что получилось](http://cssing.org.ua/examples/cssanimation), выглядит странно, но он целиком сделан на CSS! Подумать только!

Дальше, еще интересней, я [решил анимировать слова](http://cssing.org.ua/examples/cssanimation/words.html). А потом, конечно, это [случилось и с буквами](http://cssing.org.ua/examples/cssanimation/letters.html). :) Удивительно в этом то, что эту анимацию совершают всего 3-4 строки CSS-кода. (ну и джаваскрипт который предварительно раскидывает буквы по всему экрану, но это его единственная задача)

Если добавить изменение размера, [получается забавно](http://cssing.org.ua/examples/cssanimation/letters-comp-scale.html). А потом [их можно еще и крутить](http://cssing.org.ua/examples/cssanimation/letters-comp-scaledelayrotate.html) ;), тогда они похожи на муравьёв. Но с двумя лимериками уже начинает тормозить.

По дороге получился [смешной неудачный вариант](http://cssing.org.ua/examples/cssanimation/letters-comp_FAIL.html). Буквы тут довольно неуклюжие.

[Genn](http://mega.genn.org/) сделал [ASCII трибьют](http://genn.org/junk/kit.html), и [еще один](http://genn.org/junk/kit2.html), не менее клёвый. Еще [один прекрасный с отложенной анимацией](http://genn.org/junk/kit3.html) (-webkit-transition-delay). И [синяя лужа](http://genn.org/junk/kit4.html).

Может и у вас есть варианты? :)

Если у вас вдруг нет ни Сафари ни Хрома, вот видео пары анимаций:

Нравятся мне буквы

Разбросанные буквы

Пример от [Genn](http://mega.genn.org/)

### Opera & Firefox

В последних непубличных версиях этих браузеров эффекты уже работают, и вызываются соответствующими правилами -o-transform, -o-transition, -moz-transform, -moz-transition. Так что теоретически, если вы делаете эффект для сайта, правила можно продублировать с этими префиксами, авось потом заработает ;). Пока что свойства идеально деградируют в других браузерах, просто анимации нет, все происходит мгновенно. А красотами наслаждаемся в Хроме и Сафари.

Мне известно только два, не совсем бесполезных варианта использования этих свойств, вот [здесь в правой колонке внизу](http://farukat.es/) и [вот тут смешно крутятся диски](http://forabeautifulweb.com/). Но, учитывая скорую поддержку Оперы и Фаерфокса, можно придумать что-то интересное =)

### Все примеры

- [Комикс на CSS](http://cssing.org.ua/examples/cssanimation/)
- [Трибьют от Genn](http://genn.org/junk/kit.html) [и второй](http://genn.org/junk/kit2.html), а также [суперкрутой третий](http://genn.org/junk/kit3.html), и [ошеломляющий четвертый](http://genn.org/junk/kit4.html)
- [Крутящиеся буквы](http://cssing.org.ua/examples/cssanimation/letters-comp-scaledelayrotate.html), [буквы которые засасывает](http://cssing.org.ua/examples/cssanimation/letters-comp-scaleUP.html) и [поворачивающиеся буквы](http://cssing.org.ua/examples/cssanimation/letters.php), и еще [неудачный вариант](http://cssing.org.ua/examples/cssanimation/letters-comp_FAIL.html)
- [Аналоговые часы с помощью transition](http://www.fofronline.com/2009-03/an-analogue-clock-using-only-css/)

Ваш арт по теме и мнение более чем приветствуется! :)

P.S.: Лимерики взяты из журнала [Трамвай](http://tramway.msk.ru/archive.htm), автор Татьяна Петросян, [остальные тут](http://community.livejournal.com/tramway/52061.html).
