[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Telegram][icon-chat]][chat]

# OOP exercise

Тепер ви знаєте багато про JavaScript OOP. Пам'ятаєте tiny JS world? Час використовувати свою нову силу.

## Завдання 

1. Удосконалюйте свій tiny JS world model, яку ви форкнули
   [звідси](https://github.com/OleksiyRudenko/a-tiny-JS-world).
   Цього разу використовуйте свої улюблені методи JS ООП для збереження
   принципів DRY and SOLID.

   На цей раз вам не потрібен форк, працюйте з наявним репо.
   Git зберігає історію для вас.
   
   Ці [матеріали](https://github.com/OleksiyRudenko/a-tiny-JS-world/blob/master/README.md#learn-on-your-own) будуть корисні.

### Найпоширеніші проблеми для вирішення

- [ ] Якщо класи одного рівня (peer classes/siblings) мають такі самі властивості, то вони повинні бути узагальнені в їхньому базовому (батьківському) класі
- [ ] Класи для видів, які не мають рук за природним задумом - не мають рук або будь-якої еквівалентної властивості
      і не успадковують такі властивості від жодного з базових/батьківських класів
- [ ] Властивості класу, які є частинами рядка презентації об’єкта, перераховуються/вказуються явно
      (i.e. `Object` методи `values`, `keys`, `entires` або такі конструкції `for (key in obj)` не використовуються)
- [ ] Конструктор рядків презентації об’єкта є методом класу, а не незалежною функцією
- [ ] Конструктор класу визначається іменованими параметрами
- [ ] Клас не призначає і не змінює властивість, що належить будь-якому іншому класу (визначена в будь-якому іншому класі)
- [ ] Дочірній клас не повинен безпосередньо використовувати успадковану властивість для створення рядка презентації об’єкта
- [ ] Код є [OOP](https://www.freecodecamp.org/news/object-oriented-programming-concepts-21bb035f7260/), SOLID ([eng](https://medium.com/@cramirez92/s-o-l-i-d-the-first-5-priciples-of-object-oriented-design-with-javascript-790f6ac9b9fa), [rus](https://medium.com/webbdev/solid-4ffc018077da)) та [DRY](https://code.tutsplus.com/tutorials/3-key-software-principles-you-must-understand--net-25161) compliant
- [ ] Застряг або щось не зовсім зрозуміло? Задайте питання

### Перевірка коду та завершення виконання завдання

1. Для цього завдання вам знадобиться review коду:
   - Для студентів курсу **Frontend 2022**: будь ласка, дотримуйтесь [цих інструкцій](https://github.com/kottans/frontend-2021-homeworks/blob/master/README.md)
   - Для студентів **p2p course**: будь ласка, дотримуйтесь [цих інструкцій](https://github.com/kottans/frontend-2019-p2p/blob/master/CONTRIBUTING.md)
   - Зауважте, що особливо це завдання вимагає від вас подання
   один файл (`index.js` **лише**) до
   `frontend-2022-homeworks` або `frontend-2019-p2p` репозиторію для перевірки коду.
1. Чудова робота! Діліться своїми досягненнями з іншими –
   опублікувати повідомлення в [course channel][chat]:
   `OOP Exercise — #done` (або `OOP Exercise — #p2p_done` якщо ви студент курсу p2p) і додайте посилання до свого репо. **Цей крок важливий, оскільки він допомагає наставникам відстежувати ваш прогрес!**
1. Прочитайте одну-дві статті про ООП за посиланнями в
   [цьому репо](https://github.com/OleksiyRudenko/a-tiny-JS-world/blob/master/README.md#learn-on-your-own)

## Додаткові матеріали

[Fun Fun Function - Composition over Inhertance](https://www.youtube.com/watch?v=wfMtDGfHWpA)

## Готово?

➡️ Ідіть далі [Offline Web Applications](app-design-offline.md)

⤴️ Повернутися до [Contents](../contents.md)


[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg

[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome#front-end-development
[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q
