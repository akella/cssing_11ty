---
title: "Памятка по CSS layouts"
date: "2005-06-29"
humanDate: "29 Jun, 2005"
permalink: "2005/06/29/css-layout/"
tags: 
  - "common"
comments: 
  -  author: "mourner"
     id: "1938"
     url: "http://solitary.org.ua"
     date: "2005-07-07 22:38:37"
     humandate: "07 Jul, 2005"
     content: | 
       Нет, elastic-layout'ы верстать так же легко, как и фиксированные. Это просто приходит с опытом.
       
       Лично мне очень помог пост на <a href="http://www.pixelmeadow.com/blog/2005/05/25/about-elastic-layouts" rel="nofollow">www.pixelmeadow.com</a>

     email: "equimanthorn@rambler.ru"

  -  author: "Oleg"
     id: "1911"
     url: ""
     date: "2005-06-29 15:30:35"
     humandate: "29 Jun, 2005"
     content: | 
       Мне, как пользователю, нравится обыкновенный резиновый сайт, где главная колонка текста плавает с max-width:40em

     email: "oleg@subway.net.ru"

  -  author: "akella"
     id: "1912"
     url: "http://cssing.iatp.org.ua"
     date: "2005-06-29 16:10:35"
     humandate: "29 Jun, 2005"
     content: | 
       Jello + em(а не пиксели) и есть решение.
       Это был бы компромисс между полноценной резиной и фиксированными колонками.
       Просто фигово реализуются эти max-width и min-width в IE...:(

     email: "akella.a@gmail.com"

  -  author: "ganges"
     id: "1914"
     url: ""
     date: "2005-06-29 16:29:53"
     humandate: "29 Jun, 2005"
     content: | 
       Слишком много названий, имхо :) Самый в плане accessibility + visual design сайт, опятьже. имхо, - это у дагласа баумана. Мне лично еще нравится сайт Томми Ольссона.
       
       Так вот у Баумана чтоли "эластичная"? 
       
       Но для меня в последнее время важен source order более, чем то, как будет называться layout. Последовательный сорс-ордер в порядке, от главного к второстепенному, последовательность div'ов типа branding, nav, contentcontainer, siteinfooter :)
       
        а потом все это в 2 или три колонки :) с "выделкой" посредине
       а потом бодаться со шрифтами
       Проверять - мозиллой или ФФ зумминг на 200%
       Если читабельно все - значит - катит
       
       Со шрифтами у меня борьба идет постоянная :( задавать их для ИЕ надо только в % (имхо), в боди font-size:76%, если в em'ах, то потом в ИЕ колбасит
       
       В принципе, чтобы хороший нефиксированный layout сделать "под всех" - париться надо недели 2 :) Я прав?

     email: "andrey.stefanenko@gmail.com"

  -  author: "saddat"
     id: "1978"
     url: ""
     date: "2005-07-11 16:02:10"
     humandate: "11 Jul, 2005"
     content: | 
       здорово
        надо пробовать.

     email: "test@test.ru"

  -  author: "polch"
     id: "2068"
     url: "http://www.tobto.com.ua/"
     date: "2005-08-10 11:33:30"
     humandate: "10 Aug, 2005"
     content: | 
       для меня в идеале - все резиновое, но пока приходится довольствоваться "смежными" решениями, так как заказчикам не нравится ломка структуры, которая не наблюдается в таблицах. что-то обязательно должно быть с фиксированной шириной/высотой. для себя же я все делаю резиновым и не жалею :)
       
       статья супер - спасибо!

     email: "nebesna@bigmir.net"

  -  author: "memyself"
     id: "2103"
     url: "http://npj.ru/valine"
     date: "2005-08-25 10:05:58"
     humandate: "25 Aug, 2005"
     content: | 
       2mourner - весёлая статейка, особенно радует количество информации про еластик-лейауты. Ж) Шутка. Вот, перевод сделал - http://npj.ru/valine/about-elastic-layouts

     email: "val.budkin@gmail.com"

  -  author: "cssing :: Архив   :: cssing 2005"
     id: "2677"
     url: "http://cssing.org.ua/2005/12/27/cssing-highlights-2005/"
     date: "2005-12-27 14:58:12"
     humandate: "27 Dec, 2005"
     content: | 
       [...] кторов - о том какой селектор выигрывает - когда оба задают противоречивые CSS значения. Памятка по CSS layouts - обзор различных способов для построения layout страниц - то есть разметки на [...]

     email: ""

  -  author: "Mark"
     id: "4260"
     url: "http://n/a"
     date: "2006-08-11 22:36:30"
     humandate: "11 Aug, 2006"
     content: | 
       Забыл сказать, что это не фоновый рисунок для всего окна, а для для его части с фиксированной шириной, скажем, 770 пикселей, который я определяю в body.

     email: "mark.davidson@gamebox.net"

  -  author: "Mark"
     id: "4259"
     url: "http://n/a"
     date: "2006-08-11 22:33:42"
     humandate: "11 Aug, 2006"
     content: | 
       А есть ли возможность реализовать в xhtml высоту в 100%? Я хочу растянуть фоновую картинку по высоте окна вне зависимости от кол-ва контента. Пробовал сделать отдельный div c height:100%; но это не помогает :(

     email: "mark.davidson@gamebox.net"

  -  author: "akella"
     id: "4273"
     url: "http://cssing.org.ua"
     date: "2006-08-12 15:20:31"
     humandate: "12 Aug, 2006"
     content: | 
       может быть http://cssing.org.ua/2004/09/10/flex-faux/ вот эта статья прийдется вам кстати, насколько я понял не обязательно что бы колонка физически растягивалась на всю высоту, достаточно визуального эффекта который и описан в том посте.

     email: "akella.a@gmail.com"

  -  author: "fortnite account generator"
     id: "508651"
     url: "https://undana.ac.id/wp-content/uploads/fsqm-files/fortnite-account-generator.pdf"
     date: "2021-01-30 06:40:53"
     humandate: "30 Jan, 2021"
     content: | 
       Hey there! Do you know if they make any plugins to safeguard against hackers? I'm kinda paranoid about losing everything I've worked hard on. Any recommendations?|

     email: "Zsadanyi@gmail.com"

layout: "layouts/post.njk"
excerpt: "Прочитав пост на <a href=\"http://coda.co.za/\">coda.coza</a>, по адресу <a href=\"http://coda.co.za/archive/20050616/17:11:16\">http://coda.co.za/archive/20050616/17:11:16</a> , просто не могу удержаться и не \"перевести\" к себе. (никак не успеваю за своим RSS-ридером...:(). Перепись почти всех layout-техник для построения шаблонов страниц..."
---

Прочитав пост на <a href="http://coda.co.za/">coda.coza</a>, по адресу <a href="http://coda.co.za/archive/20050616/17:11:16">http://coda.co.za/archive/20050616/17:11:16</a> , просто не могу удержаться и не "перевести" к себе. (никак не успеваю за своим RSS-ридером...:(). Перепись почти всех layout-техник для построения шаблонов страниц...<!--more-->
<h3>Предисловие</h3>
Всё ниженаписанное - копия с сайта <a href="http://coda.co.za/">coda.coza</a>. Ни на какое авторство не претендую. Просто "свои" букмарки ближе к телу... ;)
<h3>Техники</h3>

1. <strong>Фиксированная</strong>: ширина колонок задана в пикселах (как правило), а ширина всей страницы такая, что помещается на экран.(800 или сейчас уже 1024 пикселов) 
За: Просто реализовать.
Против:  Обычно ломается если увеличить размер текста в броузере.
Пример: <a href="http://www.news.com/">news.com</a>, <a href="http://www.aol.com/">aol.com</a>, <a href="http://www.macromedia.com/">macromedia.com</a> (80% CSS сайтов как минимум)

2. <strong>Резиновая</strong> (aka. Fluid): ширина задается относительными величинами, обычно используют 100% что бы растянуть страничку на весь экран.
За: Приспосабливается к любой ширине экрана. Больше информации доступно без прокрутки. Гибкость и простота последующих апгрейдов.
Против: На широких экранах страдает читабельность.
Пример: <a href="http://wired.com/">wired.com</a>, <a href="http://sercotransarctic.com/">sercotransarctic.com</a>

3. <strong><a href="http://www.themaninblue.com/writing/perspective/2004/09/21/">Зависимая от разрешения</a></strong> (Resolution dependent by Cameron Adams): меняется в зависимости от размера окна броузера. При смене размера изменяется и ширина страницы. Нужен JavaScript, но без него имеем просто фиксированный layout.
За: Полный контроль за изменениями размера странички в зависимости от размера окна броузера. Гибкость.
Против: Отбирает много времени, больше головной боли.
Пример: <a href="http://www.themaninblue.com/experiment/ResolutionLayout/">пример автора</a>, <a href="http://www.rammstein.com/">rammstein.com</a>, <a href="http://www.microsoft.com/">microsoft.com</a> (для изменения нужно обновить окно).

4. <strong><a href="http://www.alistapart.com/articles/elastic/">Эластичная</a></strong> (by <a href="http://www.htmldog.com/">Patrick Griffiths</a> и недавно, <a href="http://www.456bereastreet.com/archive/200504/fixed_or_fluid_width_elastic/">Roger Johansson</a>, и опять by <a href="http://www.stopdesign.com/log/2005/06/24/zoom-layout.html?style=zoom">Douglas Bowman</a>): изменяется в зависимости от размеров шрифта пользователя. Очень похоже на зум в Опере. 
За: Пользователь может регулировать. Гибкая и доступная.
Против: Отбирает много времени, больше головной боли. Трудности с картинками.
Пример: <a href="http://www.mozilla.org/">mozilla.org</a>, <a href="http://www.yahoo.com/">yahoo.com</a>, <a href="http://www.csszengarden.com/?cssfile=/063/063.css&page=0">Elastic Lawn</a> (CSS Zen Garden)

5. <strong><a href="http://uwmike.com/archive/jello-liquid-layout/">Jello</a></strong> (by <a href="http://uwmike.com/">Michael Purvis</a>): Комбинирование Фиксированной и Резиновой техник.
За: Гибкость и простота последующих апгрейдов.
Против: не совсем простая реализация.
Пример: <a href="http://uwmike.com/layout/jello/index2.php">пример автора</a>.

6. <strong><a href="http://pro.html.it/articoli/id_620/idcat_31/pro.html">Прогрессивная</a>(?)</strong> (Progressive by Alessandro Fulciniti): Комбинация Фиксированного и Резинового.  Фиксированный - при ширине окна броузера меньше 540px (например) и больше  1024px (например); между ними - Резиновый. Требует JavaScript.(при отсутствии JS превращается в обычный Фиксированный)
За: Гибкость и простота последующих апгрейдов.
Против: не совсем простая реализация.
Пример: <a href="http://pro.html.it/esempio/proglayout/2col.html">пример автора</a>.

7. <strong>Ограниченная</strong>: Резиновая страничка с заданной максимальной шириной(в пикселах)
За: Гибкость и простота последующих апгрейдов.
Против: Использует чисто IE'шное CSS свойство для реализации max-width.
Пример: <a href="http://coda.co.za/">coda.coza</a>.
<h3>Заключение</h3>
Вот такая подборка. 
Есть на что убить пару коротких летних вечеров.
Мне лично больше всего нравится Jello, мне кажется эта техника наиболее точно отражает потребности пользователей, хотя вьехать поначалу трудновато. Но её бы я использовал для своего блога и всем рекомендовал..
ЗЫ: если для каких то из них уже общеприняты русские названия, с радостью исправлю.
