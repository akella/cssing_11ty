---
title: "Вес CSS селекторов"
date: "2005-06-09"
humanDate: "09 Jun, 2005"
permalink: "2005/06/09/css-selectors-weight/"
tags: 
  - "xhtmlcss"
  - "common"
comments: 
  -  author: "bsn"
     id: "1857"
     url: "http://www.bsn.kiev.ua"
     date: "2005-06-09 18:11:29"
     humandate: "09 Jun, 2005"
     content: | 
       отпиши что за проект. просто интересно :)

     email: "besenok@gmail.com"

  -  author: "ganges"
     id: "1858"
     url: ""
     date: "2005-06-09 22:27:48"
     humandate: "09 Jun, 2005"
     content: | 
       И пост этот писали тоже математики :) 
       Так и не понял что ты хотел этим сказать..Устал наверное (я) или вообще "дупля не отбиваю" :)
       ИМХО специфичностью большей обладает более "длинное" правило

     email: "andrey.stefanenko@gmailcom"

  -  author: "akella"
     id: "1859"
     url: "http://cssing.iatp.org.ua"
     date: "2005-06-10 10:45:50"
     humandate: "10 Jun, 2005"
     content: | 
       2 Ganges:
       Вот и я так думал... а на самом деле любой класс перешибает строку из названий 9 тэгов... По стандарту по крайней мере.
       2 bsn:
       Сервис для одного развивающегося украинского портала(какого думай сам ;) ), с перспективой на послед сотрудничество.

     email: "akella.a@gmail.com"

  -  author: "ganges"
     id: "1860"
     url: ""
     date: "2005-06-10 11:21:04"
     humandate: "10 Jun, 2005"
     content: | 
       Спасибо, теперь мне понятен смысл твоего постинга. Тогда айдишка перешибает сотню ? :))

     email: "andrey.stefanenko@gmail.com"

  -  author: "akella"
     id: "1861"
     url: "http://cssing.iatp.org.ua"
     date: "2005-06-10 11:28:34"
     humandate: "10 Jun, 2005"
     content: | 
       Я б сказал 99 ;)

     email: "akella.a@gmail.com"

  -  author: "besenok"
     id: "1862"
     url: "http://bsn.kiev.ua"
     date: "2005-06-11 12:09:22"
     humandate: "11 Jun, 2005"
     content: | 
       что за сервис ? отпиши мне на мыло пожалста

     email: "besenok@gmail.com"

  -  author: "rpuwa"
     id: "1910"
     url: ""
     date: "2005-06-29 12:24:03"
     humandate: "29 Jun, 2005"
     content: | 
       Портала, говоришь... :) Я прикололся...

     email: "grigoriy.babenko@gmail.com"

  -  author: "уке"
     id: "15348"
     url: "http://t"
     date: "2010-01-28 19:17:09"
     humandate: "28 Jan, 2010"
     content: | 
       rt

     email: "sh@mail.ru"

layout: "layouts/post.njk"
excerpt: "<strong>Оффтоп</strong>: я еще жив. :)
<strong>Оффтоп 2</strong>: PHP программерам смотреть конец поста...
Когда долго писал слoжные по логике стили иногда начинал путаться в каскадах.
Какое правило над каким имеет приоритет? Не всегда был уверен...
"
---

<strong>Оффтоп</strong>: я еще жив. :)
<strong>Оффтоп 2</strong>: PHP программерам смотреть конец поста...
Когда долго писал слoжные по логике стили иногда начинал путаться в каскадах.
Какое правило над каким имеет приоритет? Не всегда был уверен...
<!--more-->
Быть может кому то пригодится(выдержка с В3Ц):
<pre>
LI            {...}  /* a=0 b=0 c=1 -> specificity =   1 */
UL LI         {...}  /* a=0 b=0 c=2 -> specificity =   2 */
UL OL LI      {...}  /* a=0 b=0 c=3 -> specificity =   3 */
LI.red        {...}  /* a=0 b=1 c=1 -> specificity =  11 */
UL OL LI.red  {...}  /* a=0 b=1 c=3 -> specificity =  13 */ 
#x34y         {...}  /* a=1 b=0 c=0 -> specificity = 100 */ 
</pre>

Короче говоря в селекторе - каждое название тэга - <strong>1</strong> балл,
каждое название класса - <strong>10</strong> баллов,
и каждое название ID - <strong>100</strong> баллов.

Определенно, все это придумывали математики...

<h3>Работа</h3>
Разыскивается хороший <strong>киевский</strong> PHP программер для <strong>долгосрочного проекта</strong>(<strong>не</strong>благотворительного). Интересующимся слать мне мыло с указаниeм работ.  (мой адрес внизу) Или в комменты...
