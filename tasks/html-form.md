[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&emsp;
[![Telegram][icon-chat]][chat]

# Форми

## Вступ

Форми — основа вебу. Грубо кажучи, типовий застосунок здебільшого складається із форм та списків. Форми повинні бути:

- **зручними**: користувач чітко розуміє, яку дію має зробити, чи що ввести. Якщо ввід користувача неправильний, це повинно бути повідомлено в зрозумілій формі. Поля вводу і форма повинні реагувати на дії користувача надаючи чітке розуміння, що відбувається, і що потрібно зробити (чи поле активне, сфокусоване, чи очікується введення даних тощо).
- **доступними**: користувач часто заповнює форму не на комп'ютері, а на мобільному проистрої, не за допомогою мишки, а за допомогою клавіатури замість неї, іноді з допомогою зчитувача екрану. Сучасні веб-застосунки повинні бути зручними в усіх перерахованих випадках.
- гарними і **функціональними**: стандартний вигляд полів вводу може сильно відрізнятися від дизайну застосунку. Їх стилізація деяких полів може бути доволі складна, оскільки потрібно *повністю* зберігати функціональність.

Останнє часто розв'язується за допомогою JavaScript, але цей підхід має певні недоліки. Ми рекомендуємо використовувати тільки HTML і CSS. Ці дві технології надають широкий набір інструментів, щоб без значних зусиль вирішити _переважну більшість_ задач в цьому завданні, та в подібних задачах за межами курсу.

## Ключові поняття

- form
- fieldset, legend, label
- checkbox, radio button, select
- tabindex
- validation
- accessibility

<!--

I don't find this any useful despite I translated it already

## Навики, які ви відточуєте в цьому завданні

Навик | Навіщо він? |
-----------------|-----------------------|
Семантичні елементи HTML | Сементичні елементи надають можливість робити доступні та іклюзивні документи (зокрема форми) із широкою підтримкою браузерів |
Стилізування стандартних елементів | Стандартні віджети можуть відрізнятися від заданого дизайну, а також бути різними в різних браузерів. |
Перевірка коду (валідація) | Багато корисного можна дінатися перевіряючи документ автоматичними інструментами, наприклад, validator.w3.org |

-->

## Завдання

Розробити [сторінку офрмлення замовлення](https://dribbble.com/shots/1322677-Checkout-Page/attachments/186093) відовідно до макету авторства Mathieu Mayer-Mazzoli.


## Критерії

- Використовуйте HTML і CSS, не використовуйте JavaScript
- Використовуйте семантичні елементи, наприклад, `<address>`, `<section>`, `<nav>` тощо — суть завдання в тому, щоб з ними ознайомитися
- Елементи форми повинні бути клікабельні, і реагувати на дії користувача.
- Дані форми повинні перевірятися виключно інструментами HTML/CSS. 
- Елементи форми повинні бути доступними незалежно від методу вводу: миша, клавіатура, тач-девайси. Бонус — тестування за допомогою зчитувача екрану (скрінрідера).
- Вигляд повинен буди наближеним до макету.
- Перевірте результета в усіх доступних браузерах і на різних пристроях.  
- Вимкніть CSS, та перевіте вигляд свого документу без нього. Чи все працює, чи все перевіряється?
- Форма повинна мати валідний [HTML](https://validator.w3.org/) і [CSS](https://jigsaw.w3.org/css-validator/). 100% відповідності не вимагається, але перевіте, що немає помилок (попередження (warnings) допускаються, але важливо, щоб ви їх розуміли).

## Додаткові ресурси

**Зауважимо**, що список рекомендованих ресурсів доволі широкий. У вас скоріше за все не вистачить часу, щоб переглянути усе **і** виконати завдання. Пам'ятайте, що практикуватися важливіше, навіть, якщо ваше рішення при цьому не буде ідеальним. Вам не потрібно читати все зараз, сфокусуйтеся на пошуках відповідей на конкретні запитання, що виникають у вас в ході роботи.

- [HTML Forms on MDN](https://developer.mozilla.org/docs/Learn/HTML/Forms) — серія статей про різні аспекти HTML-форм
- [Native Form Validation - Part I](https://medium.com/samsung-internet-dev/native-form-validation-part-1-bf8e35099f1d)
- [Native Form Validation - Part II](https://medium.com/samsung-internet-dev/native-form-validation-part-2-552c78f563b)
- [HTML5 doctor](http://html5doctor.com/element-index/) — опис HTML-елементів з прикладами
- [Лекція про HTML by Aleksei Shvaika](https://youtu.be/Y7-0yo4KCVk?list=PLr1siHsWN79BpMXpZv0rEo0b8Wqgf9SUv) for Kottans JS course 2016
- [Inhuman UI by Vadim Makeev](https://youtu.be/KAK-WAb9vow) — розмова про доступність, і що розробниким можуть з цим зробити
- [Weblind](https://weblind.ru/) — рекомендації по розробці сайтів для людей із відхиленнями зору

## Відео

Ви можете переглянути записи наших попередніх курсів:

### Front-End Course 2022
|||
-|-
[![Віктор Якубів: Стандарт і семантика HTML][2022-html-img]][2022-html]|[Віктор Якубів: Стандарт і семантика HTML][2022-html]

### Front-End Course 2021
|||
-|-
[![Олександр Островний: HTML/CSS][2021-lesson-1-img]][2021-lesson-1]|[Олександр Островний: HTML/CSS][2021-lesson-1]
[![Олександр Островний: Зображення, форми, доступність][2021-lesson-2-img]][2021-lesson-2]|[Олександр Островний: Зображення, форми, доступність][2021-lesson-2]

### Front-End Course 2020
|||
-|-
[![First workshop HTML5 Form (1/2) - Yevhen Orlov][2020-first-workshop-1-img]][2020-first-workshop-1] | [First workshop HTML5 Form (1/2) - Yevhen Orlov][2020-first-workshop-1]
[![First workshop HTML5 Form (2/2) - Oleksandr Ostrovnyy][2020-first-workshop-2-img]][2020-first-workshop-2] | [First workshop HTML5 Form (2/2) - Oleksandr Ostrovnyy][2020-first-workshop-2]
[![Second workshop HTML5 Form - Oleksandr Ostrovnyy][2020-second-workshop-img]][2020-second-workshop]|[Second workshop HTML5 Form - Oleksandr Ostrovnyy][2020-second-workshop]
[![Third workshop HTML5 Form Wrap Up - Oleksandr Ostrovnyy][2020-third-workshop-img]][2020-third-workshop]|[Third workshop HTML5 Form Wrap Up - Oleksandr Ostrovnyy][2020-third-workshop]



[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg

[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome#front-end-development
[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q

[2022-html]: https://youtu.be/DriWt09EmEw
[2022-html-img]: https://img.youtube.com/vi/DriWt09EmEw/default.jpg

[2021-lesson-1]: https://youtu.be/xogSwtgiEJ0
[2021-lesson-1-img]: https://img.youtube.com/vi/xogSwtgiEJ0/default.jpg
[2021-lesson-2]: https://youtu.be/7Q7jEa5h3FY
[2021-lesson-2-img]: https://img.youtube.com/vi/7Q7jEa5h3FY/default.jpg

[2020-first-workshop-1]: https://youtu.be/4MYA3Nocsts
[2020-first-workshop-1-img]: http://img.youtube.com/vi/4MYA3Nocsts/default.jpg
[2020-first-workshop-2]: https://youtu.be/ZoC759dIObM
[2020-first-workshop-2-img]: http://img.youtube.com/vi/ZoC759dIObM/default.jpg
[2020-second-workshop]: https://youtu.be/eTCGaUILyzg
[2020-second-workshop-img]: http://img.youtube.com/vi/eTCGaUILyzg/default.jpg
[2020-third-workshop]: https://youtu.be/NRCvOcEuDEU
[2020-third-workshop-img]: http://img.youtube.com/vi/NRCvOcEuDEU/default.jpg
