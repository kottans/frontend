[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Telegram][icon-chat]][chat]

# Building a Tiny JS World

## Завдання

1. Створіть a tiny JS world model, дотримуючись інструкцій
   [тут](https://github.com/OleksiyRudenko/a-tiny-JS-world).
   Не забувайте, що за необхідністю, ви завжди можете перекласти англомовні матеріали за допомогою онлайн-перекладачів. 

На цьому етапі вам потрібно виконати лише частину **First approach**.
Ви повернетеся до свого Tiny JS World, щоб покращити його пізніше.
Отже, поки що обмежтеся засобами, у яких ви відчуваєте себе впевнено.

### Додаткові вимоги

- Властивості об’єкта, які є частинами рядка представлення об’єкта, мають бути явно перераховані/вказані
- `Object` методи, такі як `keys`, `values`, `entries` не слід використовувати для створення рядка презентації   об’єкта оскільки вони не гарантують певного порядку ключів/значень 
- Ваш код [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself), що означає, що коли ви бачите
   патерн у вашому коді, його слід уникати. Приклади:
  - `print(dog); print(cat); etc ... ` слід переробити, використовуючи як мінімум `Array.forEach`
  - `` `${obj.prop1}; ${obj.prop2}; ${obj.prop3};` `` (так, рядки/літерали шаблону є формою коду)
    необхідно переробити з використанням відповідних методів `Array` (ви знайдете `map` і `join` найбільш зручними)

### Перевірка коду та завершення виконання завдання

**Після завершення виконайте наступне:**

1. Для цього завдання вам знадобиться review коду:
   - Для студентів курсу **Frontend 2022**: будь ласка, дотримуйтесь [цих інструкцій](https://github.com/kottans/frontend-2021-homeworks/blob/master/README.md)
   - Для студентів **p2p course**: будь ласка, дотримуйтесь [цих інструкцій](https://github.com/kottans/frontend-2019-p2p/blob/master/CONTRIBUTING.md)
   - Зауважте, що особливо це завдання вимагає від вас подання
   один файл (`index.js` **лише**) до
   `frontend-2022-homeworks` або `frontend-2019-p2p` репозиторію для перевірки коду.
1. Чудова робота! Діліться своїми досягненнями з іншими –
   опублікувати повідомлення в [course channel][chat]:
   `A Tiny JS World — #done` (або `A Tiny JS World — #p2p_done` якщо ви студент курсу p2p) і додайте посилання до свого репо. **Цей крок важливий, оскільки він допомагає наставникам відстежувати ваш прогрес!**
1. Прочитайте одну-дві статті про ООП за посиланнями в
   [цьому репо](https://github.com/OleksiyRudenko/a-tiny-JS-world/blob/master/README.md#learn-on-your-own)

## Готово?

➡️ Ідіть далі [Object-Oriented JavaScript](js-oop.md)

⤴️ Повернутися до [Contents](../contents.md)


[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg

[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome#front-end-development
[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q
