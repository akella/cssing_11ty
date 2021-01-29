---
title: "Аякс за 30 секунд"
date: "2005-11-28"
categories: 
  - "perevod"
---

Перевожу заметку с которой я начал свое знакомство с аяксом. Находится на [сайте Rasmus'a](http://rajshekhar.net/blog) - [Rasmus' 30 second AJAX Tutorial](http://rajshekhar.net/blog/archives/85-Rasmus-30-second-AJAX-Tutorial.html). Мой вольный перевод. Вообще сам Аякс я считаю немного обманом. Многие использовали те же самые приемы задолго до того как они вдруг стали "Аяксом". И эти вещи совсем не такие сложные как многие считают. Вот простой пример из одного из моих приложений. Сначала Javascript:

function createRequestObject() {
    var ro;
    var browser = navigator.appName;
    if(browser == 'Microsoft Internet Explorer'){
        ro = new ActiveXObject('Microsoft.XMLHTTP');
    }else{
        ro = new XMLHttpRequest();
    }
    return ro;
}

var http = createRequestObject();

function sndReq(action) {
    http.open('get', 'rpc.php?action='+action);
    http.onreadystatechange = handleResponse;
    http.send(null);
}

function handleResponse() {
    if(http.readyState == 4){
        var response = http.responseText;
        var update = new Array();

        if(response.indexOf('|' != -1)) {
            update = response.split('|');
            document.getElementById(update\[0\]).innerHTML = update\[1\];
        }
    }
}

Этот код создает обьект запроса, сам запрос и функцию для его принятия и распарсивания(по названиям, собственно, нетрудно догадаться). Для использования вам нужно включить этот скрипт в вашу страницу. (`<script type="text/javascript" src="js.js"></script>`) Теперь для того чтобы послать запрос нужно его прицепить к какому-нибудь событию. Например onclick или поместив прямо в href вот так:

1. <a href="javascript:sndReq('foo')">\[foo\]</a>

Это означает что при клике на эту ссылку будет отослан вот такой запрос **rpc.php?action=foo**.

В rpc.php у вас может быть примерно такой код:

1. switch($\_REQUEST\['action'\]) {
2. case 'foo': /\*...action=foo...\*/
3. /\* **тут например запрос к базе**\*/
4. echo "foo|foo done";
5. break;
6. ...
7. }

Теперь обратим внимание на handleResponse. Оно распарсивает строку "foo|foo done" и разделяет ее по символу '|'. Причем использует то что было до '|' - как id блока в HTML, а то что после - как новый innerHTML для этого блока. В данном случае, если у вас на странице есть вот такой HTML:

1. <div id="foo">
2. </div>

То как только вы кликните на ссылку, он динамически изменится на:

1. <div id="foo">
2. foo done
3. </div>

Вот собственно и все. Остальное лишь надстройка над этим простым скриптом. Заменяйте мой простой ответ от сервера "id|text" на более богатый формат XML, и делайте запрос сложнее чем просто с одной переменной. Перед тем как вы слепо установите одну из тысяч "AJAX" библиотек попробуйте сами добавить в этот скрипт нужный вам функционал, чтобы понять как именно оно работает и усложнить его ровно настолько насколько это вам нужно. Очень часто нужно не намного больше этого моего примера.

Обобщить этот подход, например для отсылки нескольких переменных, было бы очень просто, примерно так:

1. function sndReqArg(action,arg) {
2. http.open('get', 'rpc.php?action='+action+'&arg='+arg);
3. http.onreadystatechange = handleResponse;
4. http.send(null);
5. }

А функцию handleResponse можно легко расширить для более интересных целей, чем просто замещение содержимого ДИВа.

Автор - [Rasmus](http://rajshekhar.net/blog)

### В конце

Вот такая вот статейка. На ее базе мне например хватило 2Кб скрипта для создания вот [такой вот фичи для укр.нета](http://cssing.org.ua/ajax/) ([исходники](http://cssing.org.ua/examples/jx/u-jx.rar)). Не без помощи [CB](http://sudoku.org.ua/rus/) правда. :) Джаваскриптер из меня все же слабенький. Прошу прощения за местами косноязычный перевод - я старался :). Считаю это одним из лучших тюториалов для начала работы с аяксом.

Хотя бы потому, что лично мне претит использовать все эти навороченные библиотеки. Это как использовать сложную ЦМС для сайта с 3 статическими страницами. Такие вот ассоциации. И это не говоря о пушках и воробьях.

**Ваше мнение по поводу тюториала приветствуется!**
