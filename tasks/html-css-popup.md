[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Telegram][icon-chat]][chat]

# HTML і CSS практика: Hooli-style Popup

> **Hooli** є фіктивною корпорацією від
> [Silicon Valley TV series](https://www.imdb.com/title/tt2575988/).
> Багато хто вважає, що він імітує Google або Apple.
> Hooli на [Silicon Valley famdom wiki](https://silicon-valley.fandom.com/wiki/Hooli).
> Це також представлено [on the web](http://www.hooli.xyz/).

Мета цього завдання — потренуватися в кодуванні HTML і CSS з макета. Очікується, що ви поглибите свої знання HTML і CSS і відкриєте нові невідомі раніше функції.

## Вимоги

- ніякого JavaScript, лише HTML/CSS, дозволено використання препроцесорів
- ніяких зовнішніх бібліотек чи фреймворків
- підтримка веббраузера: лише Chrome (використовуйте найновіші фічі)
- очікується, що попап матиме три стани залежно від дій користувача:
  - початковий стан: попап не видно
  - після натискання на кнопку ![popup-button](../img/popup-button.png)
    попап стає видимим або прихованим, якщо воно вже відкрите
  - натисніть кнопку "More", щоб додати ще від 3 до 10 іконок і
    робить вміст попапу доступним для скролу

## Рекомендації

- Переконайтеся, що ваша навігація побудована з усіма семантичними характеристиками [rules](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav).
- Рекомендуємо переглянути [відео](https://www.youtube.com/watch?v=E6kLaaQFctU&ab_channel=VadimMakeev) про приховування чекбоксу.
- Спробуйте стилізувати свої елементи за класами (а не за тегами HTML та ID).
- Не забудьте встановити атрибут `alt` для тегів `img` (якщо ви їх використовували).
- Немає потреби додавати багато файлів (включно з icons, gitignore, configs тощо) до вашого PR. Файлів HTML і CSS буде достатньо для перевірки вашої роботи.
- Уникайте зовнішніх скриптів для значків шрифтів.
- Перевірте свій попередній перегляд у [validator](https://validator.w3.org/).
- Переконайтеся, що ви додали порожні рядки в кожен файл зі свого PR - [reason](https://stackoverflow.com/questions/729692/why-should-text-files-end-with-a-newline).
  Якщо ви забудете додати порожній рядок у кінець файлу, GitHub покаже його:

![Missed line](https://user-images.githubusercontent.com/16196199/97906688-c123c900-1d4c-11eb-8424-75e9150b0705.png)

- Перевірте свою роботу ще раз і видаліть усі зайві коментарі зі свого коду.

## Увага

:warning: ![Google-Warning](https://place-hold.it/380x24/fff/f03c15?text=Important!+Google+may+ban+your+github+pages+domain!&bold)

Вищезазначене може статися, якщо ваш дизайн імітує компоненти чи послуги Google
оскільки вони можуть вирішити, що ви створили фішинговий сайт для крадіжки
облікові дані Google ваших відвідувачів.

Щоб уникнути цього

- НЕ використовуйте слова «google», «apple», «amazon» чи будь-якого іншого бренду в
  - назві вашого проєкту/репо
  - будь-яких url
  - будь-яких селекторах css
  - будь-яких ідентифікаторах елементів HTML (включаючи створені за допомогою JS) або в іншому місці HTML
- НЕ повторюйте дизайн Google (структуру макета, стилі тощо)
- НЕ використовуйте іконки Google

## Приклади

Вам не потрібно робити свій дизайн на 100% ідентичним прикладам нижче.
Реалізація механіки важливіша.
Використовуйте приклади для довідки.

Початковий стан: попап не видимий:

![popup-hidden](../img/popup-hidden.png)

Активний стан:

![popup-visible](../img/popup-visible.png)

Розширений набір іконок, scrollable стан:

![popup-scrollable](../img/popup-scrollable.png)

Усі інтерактивні елементи мають бути позначені як такі при наведенні (hover) миші

![popup-hover-state](../img/popup-hover.png)

Усі інтерактивні елементи повинні мати стан `:focus`.

![popup-hover-state](../img/popup-focus.png)

Ви повинні мати можливість перемикатися між усіма інтерактивними елементами, використовуючи лише клавіатуру (без миші, не забувайте про стилі для стану `:focus`)

Можете спокійно використовувати [наші іконки](https://github.com/kottans/frontend/raw/master/img/popup-icons.zip).

Ви можете опублікувати свої результати на
[GitHub Pages](https://help.github.com/articles/configuring-a-publishing-source-for-github-pages/)

**Після завершення виконайте наступне:**

1. Для цього завдання вам знадобиться review коду:
   - Для студентів курсу **Frontend 2022**: будь ласка, дотримуйтесь [цих інструкцій](https://github.com/kottans/frontend-2021-homeworks/blob/master/README.md)
   - Для студентів **p2p course**: будь ласка, дотримуйтесь [цих інструкцій](https://github.com/kottans/frontend-2019-p2p/blob/master/CONTRIBUTING.md)
1. Чудова робота! Діліться своїми досягненнями з іншими –
   опублікувати повідомлення в [course channel][chat]:
   `HTML-CSS-Popup — #done` (або `HTML-CSS-Popup — #p2p_done` якщо ви студент курсу p2p) і додайте посилання до свого репо. **Цей крок важливий, оскільки він допомагає наставникам відстежувати ваш прогрес!**

## Готово?

➡️ Ідіть далі [JavaScript Basics](js-basics.md)

⤴️ Повернутися до [Contents](../contents.md)

[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg
[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome#front-end-development
[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q
