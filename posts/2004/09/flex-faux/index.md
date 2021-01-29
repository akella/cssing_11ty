---
title: "Простой прием или колонки «одинаковой высоты»"
date: "2004-09-10"
categories: 
  - "xhtmlcss"
  - "design"
  - "useful"
---

После недавних статей [Liquid Bleach](http://www.stopdesign.com/log/2004/09/03/liquid-bleach.html) и [Sliding Faux Columns](http://www.meyerweb.com/eric/thoughts/2004/09/03/sliding-faux-columns/) захотелось это как то обобщить что ли, вобщем говоря изложить на русском. Разумеется ни в коей мере не предендуя на оригинальную идею. К тому же я не нашел перевода статьи [Faux Columns](http://www.alistapart.com/articles/fauxcolumns/) ([Dan Cederholm](http://simplebits.com/ "его сайт")) (может плохо искал?). Вот об этой простой технике и о её не менее простом продолжении и пойдет речь. Сначала понятно как всегда встала проблема.

### Проблема

Проблема встала сразу после начала активного перехода с таблиц. И заключалась в колоночном дизайне. Допустим у нас страничка состоит из двух колонок. В одной все содержание, а в другой какая-нибудь навигация (примерно как на этой самой странице). Резонным будет желание сделать их разного цвета.

Как водится колонки в "стандартном дизайне" это `div`. И если задать этот цвет прямо для _них_, то он отнюдь не продолжится до самого низа. То есть картина будет примерно такая: ![неплохо, но можно лучше](http://cssing.org.ua/pic/columns/bad.gif "неплохо, но можно лучше") Это конечно не совсем плохой вариант, но логичнее было бы сделать так: ![намного лучше](http://cssing.org.ua/pic/columns/good.gif "намного лучше")

Но кто ж сказал `div`'ам быть одинаковой высоты. Это было просто, когда были таблицы, там ячейки всегда были одинаковой высоты (в каждой строке). А с дивами было сложнее. Вот в этом и заключается проблема.

### "Фиксированное" решение

Первое решение изложил [Dan Cederholm](http://simplebits.com/ "его сайт") в своей статье на [A List Apart](http://alistapart.com/) называвшейся [Faux Columns](http://www.alistapart.com/articles/fauxcolumns/). Можете подробнее почитать там, а я изложу основной прием.

Пускай эти две колонки содержатся в `div`'e. И у этого `div`'а фиксированная ширина (как и у двух колонок, что в нем). Тогда можно использовать вот такую картинку: ![почти мой фон](http://cssing.org.ua/pic/columns/goodbg.gif "почти мой фон") (картинка немного уменьшена, на самом деле её ширина должна совпадать с шириной внешнего `div`'а). И вместе с тем такой CSS:

#внешнийДИВ{
background: #fff url(bg.gif) **repeat-y** 0 0;
}

То есть повторяем этот фоновый рисунок по вертикали для обёртывающего `div`'а, а он как раз должен содержать внутри оба наших первых блока. Таким образом создаётся эффект одинаковой высоты этих блоков. Но это все разумеется лишь для колонок фиксированной ширины.

### "Резиновое" решение

Второе решение всплыло недавно. Наверно правильно будет отнести авторство к двум людям: [Douglas Bowman](http://www.stopdesign.com/) и [Eric Meyer](http://www.meyerweb.com/). Вот они и изобрели простое решение все той же проблемы, но уже для резиновых страничек. Вот здесь их оригинальные статьи на [stopdesign.com](http://www.stopdesign.com/log/2004/09/03/liquid-bleach.html) и [meyerweb.com](http://www.meyerweb.com/eric/thoughts/2004/09/03/sliding-faux-columns/)

Основная идея использованная в этом приёме очень похожа на идею использованную все тем же Бауманом в своей статье [Sliding Doors of CSS](http://www.id-as.com/arts/ala/slidingdoors/) (на русском+ [вторая часть](http://www.id-as.com/arts/ala/slidingdoors2/)). Прием заключается в создании очень большого изображения (или двух, если дизайн из трех колонок). Картинка должна быть отчасти полностью прозрачной, а в другой части должен содержаться рисунок. Эту картинку нужно, так же как и в первом приеме, повторять вертикально (`repeat-y`).

Однако сама картинка теперь уже зависит от пропорций вашей странички. Например Мейер использовал в примерах трехколоночный дизайн. Для этого понадобились такие изображения 1000-2000.gif 2000-3000.gif. Эти картинки говорят своими названиями о _том_, где они **непрозрачны**. И использовал он разумеется дизайн, где все три колонки имеют ширину 33% от внешнего блока. Тогда нужен такой CSS:

.one {background: url(1000-3000.gif) **33%** 0 repeat-y;}
.two {background: url(2000-3000.gif) **67%** 0 repeat-y;}

[Примеры Мейера](http://www.meyerweb.com/eric/css/edge/sliding-faux/demo.html) слегка усложнены. Я например не сразу понял в чем ключ (секунд десять потерял :))(хотя то вобщем-то не примеры, а тестовый набор) Вот [мой пример](http://cssing.org.ua/examples/liquidfaux.html), он годится лишь для двухколоночного дизайна(66%/33%). Но я думаю его простота поможет кому-то лучше разобраться. Попробуйте посжимать страничку с примером. Вы должны увидеть как меняется ширина правой колонки, но пропорции их остаются прежними.

Вот это собственно и все об этой технике. Как говорит гуру (Мейер) этот трюк поддерживается хорошо. Есть какие-то мелкие глюки на Mac, но нам ли о них горевать.

### Ссылки по теме

- [Пример Мейера](http://www.meyerweb.com/eric/css/edge/sliding-faux/demo.html)
- [Мой пример](http://cssing.org.ua/examples/liquidfaux.html)
- [Liquid Bleach](http://www.stopdesign.com/log/2004/09/03/liquid-bleach.html)
- [Sliding Faux Columns](http://www.meyerweb.com/eric/thoughts/2004/09/03/sliding-faux-columns/)
- [Faux Columns](http://www.alistapart.com/articles/fauxcolumns/)