---
title: "Perl мова, 23 февраля, Киев"
date: "2008-02-25"
categories: 
  - "common"
  - "tusovka"
---

Почти случайно оказался на [интереснейшем мероприятии](http://event.perlukraine.org/upw2008/) организованном московской и киевской перловыми группами. И в частности Андреем Шитовым.

![346](/pic/upw/1.jpg)Перл там

Вообще, удивительно, но я на самом деле полтора года правил скрипты на перле, и хотя звания программист вряд ли могу удостоиться, кое-что умею. Мероприятие же было дико интересным даже и без знаний перла.

![Аудитория](/pic/upw/7.jpg)Аудитория

Средний возраст программиста на Perl довольно высокий. Начал воркшоп [Андрей Шитов](http://shitov.ru). Рассказывал обо всех изменениях, что он наблюдал в Киеве за последние два года, показал тучу классных фоток Киева, когда он только успел столько нащелкать! Вообщем, рассмешил всех =) Затем рассказал о сходствах и различиях в Perl 6 и Perl 5.10. А так же, показал замечательную презентацию на немецком, было очень забавно читать всякие "Von URL"

### Рампочта

Затем выступал Алексей Капранов, один из разработчиков почты рамблера. Как оказалось, она тоже написана на перле. Некоторые факты:

- 100 серверов
- 50 тысяч строк кода на перл
- 598 ревизий главного файла с которым взаимодействуют юзеры
- 10млн принятых писем в день, полтора миллиона отосланных. Как сказал Алексей, это обусловлено всякими форумами и одноклассниками, которые шлют уведомления про каждый пук на сайте
- 2 сисадмина и пара программистов на Перле.
- 10-15% украинских пользователей
- 25 миллионов пользователей, из них 15 миллионов активных
- 3я почта в рунете

На самом деле вся эта информация из вступления к докладу, но сам доклад был слишком перл-специфичным чтобы я о нем мог рассказать.

![Алексей Капранов](/pic/upw/11.jpg)Алексей Капранов

Потом минут 20 его пытали о технических подробностях. Надо сказать, он отвечал ничего особо не скрывая. Что весьма показательно в сравнении с некоторыми украинскими специалистами, которые еще боятся делиться знаниями =)

### Как продать Перл, доклад от portaone

Как продать ручку? Можно просто пытаться продать отличную золотую суперручку абстрактному клиенту. А можно попытаться узнать чего он хочет, и дать ему именно это. Из технических преимуществ, Андрей Жиленко упомянул такие:

- CPAN
- Понятность кода и известность языка, относительно некоторых других
- Скорость разработки

Как следствие, это влияет на бюджет и сроки. Основное ударение делалось на том, что нельзя говорить клиенту о технических преимуществах языка. Нужно понять чего хочет клиент, и сказать ему что он выиграет на его же языке. Это, собственно, относится и к веб-стандартам в полной мере. Нельзя говорить клиентам что "это правильно!".

### Укроп

Блиц доклад, Дмитрий Карасик (из Копенгагена) рассказывал об украинском языке программирования. Без лишних слов, вот кусочки кода:

![Дмитрий Карасик об УКРОП](/pic/upw/9.jpg)Дмитрий Карасик об УКРОП

Или вот подлиннее:

дiйство початок(аргументи)
	нехай у;
	доки (у = 0; y < аргументи.длина; у++) то
		якщо ( аргументи\[у\].строка == '--')
			геть;
		читай( аргументи\[у\]);
	отож
отож

Код вполне рабочий, мы даже из командной строки запустили одну из таких вот программок. Автор предлагает развить конструкции "отож", до "отожбо" и "отожбойвоно". =) [Оригинальное эссе об УКРОПе](http://mcfist.livejournal.com/12285.html), где чуть более подробная инфа и предыстория.

### Форекс

Сергей Гулько, один из разработчиков системы для Forex оговорился, что им запретили рассказывать что-либо важное. В результате рассказывал о memchached и spread. Такие штуки будут интересны только тем, кто работает с большими нагрузками, но если это так, вы просто обязаны знать эти два слова. В остальном было любопытно узнать что на форексе пользователи вообще не взаимодействуют с базой данных, только с кэшом. Memchached — для разгрузки базы данных, spread — для быстрого обмена сообщениями между серверами и не только.

Разговор плавно сполз в подробности использования spread и memcached в ПО Forex. Г-н Сережкин из Яндекс старательно выпытывал у Сергея всякие мелочи, прикрываясь "сбором статистики". Так я ему и поверил, хаха!

### [Jonathan Worthington](http://www.jnthn.net/)

Примечательно, что на воркшоп приехали люди из [Дании, Англии и Испании](http://event.perlukraine.org/upw2008/stats). В частности, Джонатан, уроженец Британии живущий в Испании, один из разработчиков компилятора для Перл 6.

![Вот как надо программить](/pic/upw/2.jpg)Вот как надо про- граммить

Еще один британец рассказывал об интеграции перлового фреймворка Catalyst и джаваскриптовой библиотеки ExtJS.

Конференцию завершили докладом для начинающих программистов, "Perl 6 Tutorial". Андрей Шитов и Джонатан по очереди рассказывали о циклах, ООП, новых бинарных операторах и всем-всем-всем из Перл 6. Вышло очень динамично и интересно. В некоторые моменты запускался компилятор и начинался отлов ошибок в коде =). Особенно запомнился некто, несколько раз задавший вопрос: "Это ошибка исполнения или компиляции?". На который никто не мог никак ответить, без самого компилятора.

![Андрей Шитов и Jonathan Worthington](/pic/upw/3.jpg)Worthi- ngton & Shitov

![Андрей Шитов](/pic/upw/4.jpg)Андрей Шитов

![Jonathan Worthington](/pic/upw/6.jpg)Jonathan Worth- ington

### В конце

Вообще, на такие мероприятия опасно ходить, можно начать забывать про HTML и писать на Perl...

- [Український воркшоп «Перл мова» — 2008](http://event.perlukraine.org/upw2008/) - официальный сайт
- [Другие воркшопы по перлу](http://perl.lv/)
- [Видео с мероприятия (и я засветился, с незнакомым мне голосом)](http://event.perlukraine.org/upw2008/media/video.html)

За все фото огромное спасибо [Андрею Шитову](http://www.shitov.ru/)! =) Другие организаторы тоже постарались на славу! Все вышло без сучка и без задоринки.

Радует тенденция, в Украине и России все больше и больше таких вот качественных воркшопов-тусовок.