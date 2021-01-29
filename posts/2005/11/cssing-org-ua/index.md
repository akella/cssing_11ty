---
title: "cssing.org.ua"
date: "2005-11-10"
categories: 
  - "common"
---

Переехал. Хостинг стал напрягать своими проблемами. Надеюсь здесь будет намного уютнее :). Кроме того тот хостинг грешил медлительностью для неукраинцев - узкий канал. Тут вроде ровнее. (Менять айпишник на cssing.iatp.org.ua мне "типа" отказали.) Для переезда использовал мод\_реврайт, надеюсь это окажется кому-то полезным.

1. Options -Indexes +FollowSymLinks
2. <IfModule mod\_rewrite.c>
3. RewriteEngine On
4. RewriteCond %{HTTP\_HOST} cssing\\.iatp\\.org\\.ua$ \[NC\]
5. RewriteRule ^(.\*)$ http://cssing.org.ua/$1 \[R\]
6. RewriteRule ^(.\*)$ http://cssing.org.ua/$1 \[R=301,L\]
7. </IfModule>

([позаимствовал](http://lvm.converters.ru/93/ru/article_210.html)) Можно и более простым способом(спасибо [zaARTix](http://zaartix.ru/)):

1. Options -Indexes +FollowSymLinks
2. <IfModule mod\_rewrite.c>
3. Redirect permanent / http://cssing.org.ua/
4. </IfModule>

А работает тут все явно быстрее :). Tnx 2 **Vitos** :).

Просьба всех кто ссылается поменять ссылку на меня в блогроллах - буду возвращать PR...
