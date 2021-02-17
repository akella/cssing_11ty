---
title: "Маленькая проблемка"
date: "2004-07-28"
humanDate: "28 Jul, 2004"
permalink: "2004/07/28/small-problem/"
tags: 
  - "xhtmlcss"
  - "design"
layout: "layouts/post.njk"
excerpt: "В процессе написания стилей для этой страницы у меня возникла проблема ( с кем бы вы думали?) с IE 5.0.Я надеюсь тот простой выход что я нашел принесет кому то пользу...
"
---

В процессе написания стилей для этой страницы у меня возникла проблема ( с кем бы вы думали?) с IE 5.0.Я надеюсь тот простой выход что я нашел принесет кому то пользу...
<!--more-->

Я хотел, что бы заголовки постов на главной странице были немного смещены влево по отношению к содержанию.Мне кажется , что так легче визуально разделять страницу.
К тому же хотелось впихнуть в начало заголовка соответствующую иконку (вы могли её заметить на главной странице).Вот такую <img src="pic/ent.gif" alt="entry" title="иконка" width="16px" height="17px"  />.
Для этого я применил к заголовку такие стили:<pre>.storytitle {
        border-bottom: dotted 1px #aaa;
	font-weight:normal;
	margin-top: 0;
	padding-left:20px;
        <strong>position:relative;
	left:-1em;</strong>
	background: transparent<span class="linewrap">&#187;</span>
        url(pic/ent.gif) no-repeat left;
 }</pre>
И все бы прекрасно.FireFox , Opera и IE 6 довольны.<strong>Но</strong>.Мне пришла ,наверно,самая глупая идея которая приходит на ум верстальщику &mdash; потестировать в IE 5.0.
Вот что я увидел вместо своих желанных заголовков с отступом от текста:
<img class="bord" src="/pic/bok.gif" width="222px" height="84px" alt="IE 5 во всей своей красе" title="IE 5 во всей своей красе" />
После коротких игр  с <acronym title="Cascading Style Sheets">CSS</acronym> я понял что это не я наглючил, а майкрософт (это не я модный , это они не очень :)) .
После указания <code>position:relative;</code> IE 5.0 игнорировал мои потуги с <code>padding</code>.
В конце концов утешение я нашел в отрицательных <code>margin</code>'ах.
Поменяв старые правила для заголовков на эти :<pre>.storytitle {
	border-bottom: dotted 1px #aaa;
	font-weight:normal;
	margin-top: 0;
	padding-left:20px;
	background: transparent<span class="linewrap">&#187;</span>
        url(cssing/ent.gif) no-repeat left;
	<strong>margin-left:-1em;</strong>
}</pre>
В результате все остались довольны.И вот что стал теперь показывать IE 5.0:
<img class="bord" src="/pic/nebok.gif" width="227px" height="88px" alt="Довольный IE 5" title="Довольный IE 5" /><br />
Вот такое решение маленькой проблемки.
Похожую тему недавно обсуждали на <a href="http://www.umade.ru/">Umade</a>.
Довольно красивый и полезный русский блог.Недавно кстати <a href="http://www.umade.ru/log/2004/07/36.html">занесенный</a> в раздел noteworthy на <a href="http://www.cssvault.com/noteworthy/2004/07/index.php">CSS Vault</a> .
А это ссылка на похожую <a href="http://www.umade.ru/log/2004/07/35.html">тему</a> на Umade.
