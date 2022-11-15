[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&emsp;
[![Telegram][icon-chat]][chat]

# Форми

## Вступ

Форми — основа вебу. Грубо кажучи, типовий застосунок здебільшого складається із форм та списків. Форми повинні бути:
- **зручними**:
- usable: the user should understand clearly what action/input is required. If the user's input is incorrect, he/she should be notified in a friendly manner about it. The form should respond to user actions and give adequate feedback: user must understand what is happening and what he/she is expected to do (if the form is active, clicked, expecting input etc.)
- **доступними**:
- accessible: often the user is using a form not on desktop browser, but on a mobile device, not with a mouse, but with keyboard instead of mouse, with screen reader or other assistive device. Modern web applications are expected to provide optimal user experience in all those cases.
- гарними і **функціональними**:
- pretty and design-conform - the look of standard input widgets may diverge significantly from application design. Styling widgets is complicated, because you need to preserve functionality of a widget.

Добре, що HTML надає розробникам широкий набір інструментів, щоб 
Good news is that HTML5 provides developers with a rich set of tools to approach those challenges in an elegant way. Bad news is that not all browsers support all HTML5 goodies.
Tasks described in this lesson are often solved with JavaScript, but this approach has some downsides. It is advisable to use all possibilities of pure HTML & CSS before reaching out to JS.

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

Розробити сторінку відовідно до макету:

<figure>
    <a href="https://dribbble.com/shots/1322677-Checkout-Page/attachments/186093">
        <img src="https://cdn.dribbble.com/users/76090/screenshots/1322677/attachments/186093/checkout-preview_2x.png" alt="Попередній перегляд макету" style="width: 100%; max-height: 80vh; object-position: top; object-fit: cover;">
    </a>
    <figcaption>Checkout Page, автор Mathieu Mayer-Mazzoli</figcaption>
</figure>


## Критерії

- Використовуйте HTML і CSS, не використовуйте JavaScript
- Використовуйте семантичні елементи, наприклад, `<address>`, `<section>`, `<nav>` тощо - суть завдання в тому, щоб ознайомитися з усіма доступними орціями
- Елементи форми повинні бути клікабельні, і respond to user action.
- Дані форми повинні перевірятися виключно інструментами HTML/CSS. 
- Елементи форми повинні бути доступними незалежно від методу вводу: миша, клавіатура, тач-девайси. Бонус — тестування за допомогою зчитувача екрану (скрінрідера).
- Вигляд повинен буди наближеним до макету.
- Перевірте результета в усіх доступних браузерах і на різних пристроях.  
- Вимкніть CSS, та перевіте вигляд свого документу без нього. Чи все працює, чи все перевіряється?
- Форма повинна мати валідний [HTML](https://validator.w3.org/) і [CSS](https://jigsaw.w3.org/css-validator/). 100% відповідності не вимагається, але перевіте, що немає помилок (попередження (warnings) допускаються, але важливо, щоб ви їх розуміли).

## Додаткові ресурси

Note: The list of recommended resources is extensive. You may not have enough time to read/watch everything AND do the task. Remember, that doing the task is more important, even if the solution is not perfect. You don't need to read everything right now, concentrate on finding answers to particular questions.

- [HTML Forms on MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms) - a series of articles on different aspects of web forms
- [Native Form Validation - Part I](https://medium.com/samsung-internet-dev/native-form-validation-part-1-bf8e35099f1d)
- [Native Form Validation - Part II](https://medium.com/samsung-internet-dev/native-form-validation-part-2-552c78f563b)
- [HTML5 doctor](http://html5doctor.com/element-index/) - HTML5 elements description with examples
- [Lecture on HTML by Aleksei Shvaika](https://youtu.be/Y7-0yo4KCVk?list=PLr1siHsWN79BpMXpZv0rEo0b8Wqgf9SUv) for Kottans JS course 2016
- [Inhuman UI by Vadim Makeev](https://youtu.be/KAK-WAb9vow) - talk on accessibility and what web developers can do about it
- [Weblind](https://weblind.ru/) - Recommendations on site development for people visually impaired

## Відео

You can watch related screencasts from Kottans course live workshops below.

|||    
--- | --- 
[![First workshop HTML5 Form (1/2) - Yevhen Orlov][first-workshop-1-img]][first-workshop-1] | [First workshop HTML5 Form (1/2) - Yevhen Orlov][first-workshop-1]
[![First workshop HTML5 Form (2/2) - Oleksandr Ostrovnyy][first-workshop-2-img]][first-workshop-2] | [First workshop HTML5 Form (2/2) - Oleksandr Ostrovnyy][first-workshop-2]
[![Second workshop HTML5 Form - Oleksandr Ostrovnyy][second-workshop-img]][second-workshop]|[Second workshop HTML5 Form - Oleksandr Ostrovnyy][second-workshop]
[![Third workshop HTML5 Form Wrap Up - Oleksandr Ostrovnyy][third-workshop-img]][third-workshop]|[Third workshop HTML5 Form Wrap Up - Oleksandr Ostrovnyy][third-workshop]



[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg

[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome#front-end-development
[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q

[first-workshop-1]: https://youtu.be/4MYA3Nocsts
[first-workshop-1-img]: http://img.youtube.com/vi/4MYA3Nocsts/default.jpg
[first-workshop-2]: https://youtu.be/ZoC759dIObM
[first-workshop-2-img]: http://img.youtube.com/vi/ZoC759dIObM/default.jpg
[second-workshop]: https://youtu.be/eTCGaUILyzg
[second-workshop-img]: http://img.youtube.com/vi/eTCGaUILyzg/default.jpg
[third-workshop]: https://youtu.be/NRCvOcEuDEU
[third-workshop-img]: http://img.youtube.com/vi/NRCvOcEuDEU/default.jpg
