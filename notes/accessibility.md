Доступність
=

ARIA-атрибути
-

### `role`

Визначають структуру документа, типи віджетів тощо.

**Користуйтеся семантичними HTML-елементами**,
і вам ніколи не треба буде цей атрибут.

Детальніше: [WAI-ARIA Roles](https://developer.mozilla.org/docs/Web/Accessibility/ARIA/Roles) на MDN

### `tabindex`

Впливає на порядок переходу по елементах натисканням клавіші <kbd>Tab</kbd>

- `tabindex=-1` не дозволяє фокусувати елемент з клавіатури.
- `tabindex=0` означає, що він буде фокусуватися в порядку появи в HTML-коді
- `tabindex=<+int>` вказує конкретний порядок фокусу

Якщо ви не пишете віджет на JS, то порядок фокусування вам не треба.


### `aria-hidden`

Не може бути пустим, або `true` або `false`.
Відповідно, відображає або приховує елемент із дерева доступності.



### `aria-label`, `aria-labelledby`, `aria-description`, `aria-describedby`

Якщо в елемента немає _label_'а,
`aria-label` дозволяє його задати.
Наприклад, для гіперпосилання у вигляді іконки:

```html
<a href=https://huggingface.co aria-label="Hugging face">🤗</a>
```

Якщо візуальний _label_ є, то варто скористатися `aria-labelledby`,
вказуючи в значенні ID елемента, який описує даний інтерактивний елмент.
Наприклад:

```html
Почитати про <span id=resource-name>Hugging Face</span>
можна <a href=https://huggingface.co>тут</a>.
```

Ніколи не робіть так ☝️, робіть отак 👇

```html
Дізнайтеся більше про ресурс на сторінці
<a href=https://huggingface.co>Hugging Face</a>.
```

---

`aria-description`, `aria-describedby` працюють аналогічно,
але додають опис, а не заголовок.

Якщо опис видимий на сторінці, використовуйте `aria-describedby`.
Якщо краще, щоб опис можна було побачити, використовуйте `title`.

### `aria-live`

Три можливох значення:

- `off` (за промовчанням) — ніколи не оголошувати зміни
- `polite` — оголосити зміни, коли користувач не зайнятий (не друкує, не читає)
- `assertive` — оголосити відразу (перебиваючи читання тощо)

Керуйтеся двома правилами:

1. Не робіть «живих» елементів
2. Якщо треба живий контет, наприклад, спливаюче вікно пошуку, використовуйте `polite`

### `aria-pressed`, `aria-selected` та інші

`aria-pressed` використовується для того, щоб позначити кнопку натиснутою.
Наприклад, для [доступного переключателя](https://inclusive-components.design/toggle-button/) на базі `<button>`

`aria-selected` для позначення обраних елементів у кастомну `<select>`

---

Про ці та інші ARIA-атрибути можна [почитати на MDN](https://developer.mozilla.org/docs/Web/Accessibility/ARIA/Attributes).


Корисні ресурси
-

- [Quick Reference: How to Meet WCAG](https://www.w3.org/WAI/WCAG21/quickref/)
- [WAI-ARIA Authoring Practices 1.2](https://w3c.github.io/aria-practices/)
- [Inclusive Components](https://inclusive-components.design/)
