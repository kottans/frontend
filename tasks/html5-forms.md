[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Telegram][icon-chat]][chat]

### HTML5: Forms
#### Intro

Forms are the very essence of web. Roughly speaking an average web application consists mostly of forms and lists. Forms are expected to be:
- usable: the user should understand clearly what action/input is required. If the user's input is incorrect, he/she should be notified in a friendly manner about it. The form should respond to user actions and give adequate feedback: user must understand what is happening and what he/she is expected to do (if the form is active, clicked, expecting input etc.)
- accessible: often the user is using a form not on desktop browser, but on a mobile device, not with a mouse, but with keyboard instead of mouse, with screen reader or other assistive device. Modern web applications are expected to provide optimal user experience in all those cases.
- pretty and design-conform - the look of standard input widgets may diverge significantly from application design. Styling widgets is complicated, because you need to preserve functionality of a widget.

Good news is that HTML5 provides developers with a rich set of tools to approach those challenges in an elegant way. Bad news is that not all browsers support all HTML5 goodies.
Tasks described in this lesson are often solved with JavaScript, but this approach has some downsides. It is advisable to use all possibilities of pure HTML & CSS before reaching out to JS.

#### Key Terms

- Form, widget
- fieldset, legend, label
- checkbox, radio button, select
- tabindex
- validation
- accessibility

#### Skills to master in this lesson

Skill/Competence | Why shold I learn it? |
-----------------|-----------------------|
HTML5 semantic elements | HTML5 semantic element provide developers with rich possibilities to develop usable, accessible forms with good browser support |
Styling built-in elements | Native widgets may not match the design. also the look of a widget may differ between browsers. |
HTML5 validation | Many useful validations can be done with native HTML validation |

#### Task Description

Make a form according to mockup: https://dribbble.com/shots/1322677-Checkout-Page/attachments/186093

##### Acceptance criteria

- Use only HTML & CSS, no JavaScript.
- Use semantic HTML elements like `<address>`, `<section>`, `<nav>` etc. - this task's purpose is to showcase all the available options and make you familiar with them.
- Form elements should be clickable and respond to user action.
- Form data should be validated using HTML/CSS capabilities only. 
- Form elements should be accessible via any type of input: mouse, keyboard, touch devices. Bonus points for testing with screen readers.
- The look should be as close as possible to mockup.
- Test the result in all available browsers & on different devices.  
- Turn off CSS styling and check how your form looks and if it is still usable (and validated properly).
- Form should be tested for valid [HTML](https://validator.w3.org/) & [CSS](https://jigsaw.w3.org/css-validator/). 100% compliance is not required, but make sure you don't have errors (warnings are acceptable, just make sure you understand them).

#### Resources

Note: The list of recommended resources is extensive. You may not have enough time to read/watch everything AND do the task. Remember, that doing the task is more important, even if the solution is not perfect. You don't need to read everything right now, concentrate on finding answers to particular questions.

- [HTML Forms on MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms) - a series of articles on different aspects of web forms
- [Native Form Validation - Part I](https://medium.com/samsung-internet-dev/native-form-validation-part-1-bf8e35099f1d)
- [Native Form Validation - Part II](https://medium.com/samsung-internet-dev/native-form-validation-part-2-552c78f563b)
- [HTML5 doctor](http://html5doctor.com/element-index/) - HTML5 elements description with examples
- [Lecture on HTML by Aleksei Shvaika](https://youtu.be/Y7-0yo4KCVk?list=PLr1siHsWN79BpMXpZv0rEo0b8Wqgf9SUv) for Kottans JS course 2016
- [Inhuman UI by Vadim Makeev](https://youtu.be/KAK-WAb9vow) - talk on accessibility and what web developers can do about it
- [Weblind](https://weblind.ru/) - Recommendations on site development for people visually impaired


[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg

[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome#front-end-development
[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q
