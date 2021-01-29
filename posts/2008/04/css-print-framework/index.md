---
title: "CSS print framework"
date: "2008-04-07"
categories: 
  - "xhtmlcss"
  - "useful"
---

Пафосное название для моего обычного стандартного print.css который я всюду инклюдю. Несколько общих правил для печатных стилей, которые будет легко дополнить своими.

Разумеется, по-хорошему, каждый проект нуждается в своем печатном стиле. Но, на деле, когда вы верстаете 10 (вы монстр!) сайтов в неделю, такой вот шаблон print.css становится приятным бонусом, и знаком вашего профессионализма.

Файл состоит из нескольких условных групп правил. Сложного нет ничего. Просто экономлю мировую энтропию, чтобы кто-то не парился и украл у меня этот файл. =)

### Общие стили

Шрифты и цвета. При печати лучше смотрится черный на белом, и текст с засечками:

1. body {
2. margin:.2in .55in; /\*отступы от края страницы, для красоты\*/
3. padding:0;
4. background:#fff;
5. color:#000;
6. font:12pt "Times New Roman", Garamond, serif;/\*шрифт с засечками\*/
7. }
8. form,  
    #secondary,  
    #sidebar,  
    #nav,  
    #whatever {/\*прячем ненужные при печати блоки, единственная часть печатного файла которую нужно обновлять на новом проекте\*/
9. display:none;
10. }

В каждом проекте свои блоки нужно скрывать и показывать, все же остальные правила остаются неизменными.

### Текст

Самые обычные приятные отступы и размеры. h1 самый большой, h2 поменьше, h3 еще меньше. И все прижимаются к тексту (margin-bottom:0):

1. h1, h2, h3 {
2. margin:.6em 0 0 0;
3. font-family:Georgia,Serif;
4. font-weight:normal;
5. clear:both;
6. }
7. h2 {
8. font-size:240%;
9. margin:.3em 0 0 0;
10. }
11. ...
12. h3+blockquote,  
    h2+blockquote,  
    p+ul{ /\*между заголовком и абзацем лучше иметь минимальный отступ\*/
13. margin-top:.2em;
14. }

### Ссылки

Псевдоселектор `:after`, работает только в "хороших" броузерах. В результате, в печати после текста ссылки добавляет её URL в скобочки.

![УРЛ в скобочках](http://cssing.org.ua/pic/url.png)URL

Вот, css-magic:

1. #content a\[href\]:after {
2. content: " (" attr(href) ") ";
3. font-size: 90%;
4. }
5. #content a\[href^="/"\]:after{/\*для ссылок вроде href="/feed/"\*/
6. content: " (http://cssing.org.ua/" attr(href) ") ";
7. }
8. abbr:after,  
    acronym:after {/\* аббревиатуры \*/
9. content: " ("attr(title)") ";
10. }

### Результат

Этих стилей достаточно, чтобы ваша страничка начала печататься примерно так:

[![скриншот версии для печати](http://cssing.org.ua/pic/cssingprint.png)Версия для печати (pdf, 160Kb)](http://cssing.org.ua/pic/cssing.pdf)

Мне, очень нравится. Все что нужно дальше, легко добавить в этот фреймворк. Но базу он задает. Обожаю маленькие фреймворки!

### Читать дальше

- [Мой CSS print фреймворк](http://cssing.org.ua/pic/print.css) (осторожно! размер файла 1.3Kb)
- [CSS Design: Going to Print](http://www.alistapart.com/stories/goingtoprint/)
- [CSS Styling for Print and Other Media](http://www.digital-web.com/articles/css_styling_for_print_and_other_media/)
- [Printing the Web: Solutions and Techniques](http://www.smashingmagazine.com/2007/02/21/printing-the-web-solutions-and-techniques/)

- [На New York Times, кстати продают](#) [места в печатной версии](http://www.nytimes.com/2008/04/07/world/middleeast/07iraq.html?_r=1&hp=&oref=slogin&pagewanted=print) (вверху справа) :)
- [Печатные стили для CSSing](http://cssing.org.ua/wp-content/themes/cssing2/css/print.css) — типичный пример моего фреймворка в работе, добавлено несколько специфических правил для блога
- [Подбор материалов c семинара npj](http://npj.ru/seminar/printversion/) — очень всеобъемлющий материал, несмотря на возраст.
- [Javascript для вынесения ссылок из текста в конец печатной версии](http://designformasters.info/posts/improving-link-display-for-print/)
- [Замена :after для IE (expression), нюанс — нет скобочек](http://elv1s.ru/files/js/ie-content-after.html)

Буду рад если поделитесь своими советами и печатными хаками. С радостью внесу в этот файл, чтобы он был еще более полезным!
