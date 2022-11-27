Компонування, чи «лейаути»
=


Responsive vs Adaptive Layouts
-

![Responsive Layout on the left vs Adaptive Layout on the right](https://www.springboard.com/blog/wp-content/uploads/2021/05/Responsive-vs-Adaptive-Web-Design.png)

|Responsive|Adaptive|
|----------|--------|
|**Розтягується** в залежності від доступного простору|**Перебудовується** в залежності від доступного простору|


### Mobile First

Філософія дизайну, яка полягає в дизайні для мобільних пристроїв в першу чергу.
Можна трактувати це, як підхід до структурування інформації в дизайні:
спочатку найважливіше, все, що влазить на найменший екран,
і поступово додається більше деталей зі збільшенням розміру екрану.

Не зважаючи на те, що тема чомусь дуже роздута,
не дуже є сенс перетягувати її в front end,
бо часто реалізація інтерфейсу відмінна від того, як він проєктується.

Філософія бере свій початок з Google, де їм було важливо зробити сайти кращими
для користувачів, які почали масово приходити з мобільних пристроїв.
Першим її [презентував Luke Wroblewski](https://youtu.be/kLLNrVodDq4) в 2011 році.

Якщо коротко про mobile first у front end'і,
то це написання медіазапитів ширини екрану виключно у форматі:

```css
@media (min-width: 600px) {}
@media (min-width: 960px) {}
```

тощо, і **не мати** запитів вигляду:

```css
@media (min-width: 640px) and (max-width: 1280px) {}
@media (max-width: 600px) {}
```


### Media Queries

Якщо говорити про запити до розміру екрану, то чим їх менше —
тим легше підтримувати такий код. Старайтеся їх мінімузвати.

Стосовно запитів, таких як
`orientation`,
`prefer-reduced-motion`,
`prefer-color-scheme`,
`hover` тощо,
залежить від ваших побажань щодо доступності.

[Список усіх доступних речей, які можна перевірити медіа-запитом](https://developer.mozilla.org/en-US/docs/Web/CSS/@media#media_features) на MDN


Grid ~vs~ and Flexbox
-

[![One-dimentional flexbox, two-dimentional grid](https://ishadeed.com/assets/grid-flex/grid-vs-flexbox.png)](https://ishadeed.com/article/grid-layout-flexbox-components/)

Джерело: [Grid for layout, Flexbox for components](https://ishadeed.com/article/grid-layout-flexbox-components/), Ahmad Shadeed


### Flexible box

|Вісь|`flex-direction: row`|`flex-direction: column`|
|----|---------------------|------------------------|
|Головна|![Головна вісь, row](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox/basics1.png)|![Головна вісь, column](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox/basics2.png)|
|Перехресна|![Перехресна вісь, row](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox/basics3.png)|![Перехресна вісь, column](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox/basics4.png)|

Головна вісь залежить від `flex-direction`,
який в свою чергу _залежить від `writing-mode`_.

Поперечна вісь завжди перпендикулярна до головної.

Початок і кінець головної, а також поперечної осі, залежить від напрямку тексту.

Дві властивості, які вам найчатіше треба будуть:
`flex-wrap: wrap` (коли треба `flex-direction: row`)
та `flex-direction: column` (в іншому випадку).
Можливість блоків «перестрибувати», коли їм не вистачає місця,
якраз і робить їх «гнучкими».

- [Basic concepts of flexbox](https://developer.mozilla.org/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox)
- [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/), Chris Coyier для CSS Tricks
- [What the Flexbox](https://flexbox.io), Wes Bos
- [An Interactive Guide to Flexbox](https://www.joshwcomeau.com/css/interactive-guide-to-flexbox/), Joshua Comeau

### Grid

- [Grid на MDN](https://developer.mozilla.org/docs/Web/CSS/CSS_Grid_Layout)
- [A Complete Guide to CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/), Chris House для CSS Tricks
- [Things I’ve Learned About CSS Grid Layout](https://css-tricks.com/things-ive-learned-css-grid-layout/), Ollie Williams для CSS Tricks
- [Grid by Example](https://gridbyexample.com/examples/)

### Модульна сітка на 12 колонок

Не треба.

<details>
<summary>Чому?</summary>

[Модульні сітки](https://uk.wikipedia.org/wiki/Модульна_система_верстки) — це метод графічного дизайну,
який допомагає компонувати контент в певному чітко окресленому просторі,
наприклад, сторінці книги, газети, плакаті, тощо.

Коли почав зароджуватися веб-дизайн, різноманіття екранів не було,
та й ця сфера не могла зародитися нізвідки,
а почала базуватися на типографічному дизайні.

Модульна сітка на 12 рівних колонок історично стала найбільш гнучкою моделлю
для дизайну того, що ти поки не знаєш, як робити:
вона легко ділиться на дві, три чи чотири рівні колонки,
одну менщу й одну більшу, дві вужчі й одну широку тощо.
В результаті творчого процесу з 12-модульної сітки
утворюється макет на потрібну кількість колонок
та виділені місця для певного типу вмісту (зображення, текст, заголовки).

Процес дизайну у вебі може бути подібним.
Але це не є процесом верстки.
На вeрстку отримується макет із уже чітко визначеними областями контенту,
не важливо, чи для їх утворення була використана 12-модульна сітка, чи ні.
В сучасних реаліях це ускладнується ще й різноманіттям розмірів екранів:
для малих дисплеїв це може бути 1–4 модулі,
для більших — 4–12, а то й 24!
Приклад: [модульні сітки Material Design 2](https://m2.material.io/design/layout/responsive-layout-grid.html#columns-gutters-and-margins).

Як розробникам, вам не треба вдаватися в концепти мислення дизайнера,
коли ви верстаєте сторінку,
хоча корисно знати базові принципи дизайну для взаємопорозуміння з колегами.
Вам треба всього лише передавати дизайн на практиці так,
щоб він відображав задум автора.
Зазвичай це доступність:
текст має бути читабельний, не надто широкий, не надто вузький,
зображення має бути чітким, розтягуватися до країв, не бути під текстом тощо.

Це так в ідеальному світі, коли ви працюєте з кваліфікованими дизайнерами.
Не всі мають високу кваліфікацію, тому дивіться по ситуації.

<details>
<summary>Як зробити?</summary>

Короткий приклад:

```css
.grid {
	display: grid;
	grid-template-columns: repeat(12, 1fr);
	gap: 1rem;
}

.grid-col-5 {
	grid-column: auto / span 5;
}

.grid-col-7 {
	grid-column: auto / span 7;
}

.grid-start-1 {
	grid-column-start: 1;
}


.grid-start-7 {
	grid-column-start: 7;
}

/* І так для всіх 12 */
```

Реальний приклад — Bootstrap:

- [Бібліотека](https://github.com/twbs/bootstrap/blob/main/scss/mixins/_grid.scss)
- [Сітка](https://github.com/twbs/bootstrap/blob/main/scss/_grid.scss)

</details>

</details>


Методи макетування
-

1. `margin-*: auto` займає весь доступий простір в лінійній осі
2. `flex-basis` вказує _ідеальний_ розмір для блока
3. `flex-basis` буде проігнорований, коли має від'ємне значення


### Центрування по горизонталі

```css
.center {
	padding: 1rem;
	margin-inline: auto;
	max-inline-size: 80ch;
}
```

### Центрування по вертикалі

```css
.centered-vertically {
	display: flex;
	flex-direction: column;
	justify-content: center;
}
```

Це один з прикладів, але є ще багато [трюків від W3C](https://www.w3.org/Style/Examples/007/center.en.html).


### Stack

```css
* {
	margin-block: 0;
}

* + * {
	margin-block-start: 1rem;
}
```

Джерело: [Every Layout](https://every-layout.dev/layouts/stack/)


### Sidebar

```css
:has(> .sidebar) {
	display: flex;
	flex-wrap: wrap;
	gap: 1rem; /* optional */
}

:has(> .sidebar) > :where(:not(.sidebar)) {
	flex-basis: 0;
	flex-grow: 999;
	min-inline-size: 50%;
}

.sidebar {
	flex-basis: 20rem; /* бажаний розмір сайдбара */
	flex-grow: 1;
}
```

Джерело: [Every Layout](https://every-layout.dev/layouts/sidebar/)


### Switcher

```css
.switcher {
	--breakpoint: 30rem;

	display: flex;
	flex-wrap: wrap;
	gap: 1rem; /* optional */
}

.switcher > * {
	flex-grow: 1;
	flex-basis: calc((var(--breakpoint) - 100%) * 999);
}
```

Джерело: [Flexbox Holy Albatross](https://www.youtube.com/watch?v=RUyNJaoJH_k), Haydon Pickering, CSS Day 2019


### Grid

```css
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(15rem, 1fr));
  gap: 1rem; /* optional */
}
```

Джерело: [A Deep Dive Into CSS Grid `minmax()`](https://ishadeed.com/article/css-grid-minmax/), Ahmad Shadeed


### Hidden, hidden visually

Приховує елемент повністю:

```css
[hidden] {
	display: none !important;
}
```

`!important` небхідний для того,
щоб 100% перекрити `display` складних селекторів вагою більше 1 класу.

Приховує елемент, але залишає його доступним для зчитувачів екрану.

```css
.visually-hidden,
.visually-hidden-focusable:not(:focus):not(:focus-within) {
	position: absolute !important;
	width: 1px !important;
	height: 1px !important;
	padding: 0 !important;
	margin: -1px !important;
	overflow: hidden !important;
	clip: rect(0, 0, 0, 0) !important;
	white-space: nowrap !important;
	border: 0 !important;
}
```

Джерело: [Bootstrap](https://github.com/twbs/bootstrap/blob/main/scss/mixins/_visually-hidden.scss), [The Accessibility Project](https://www.a11yproject.com/posts/how-to-hide-content/)


Як ресетити стилі
--

Ось кілька варіантів:

|[reset.css](http://html5doctor.com/html-5-reset-stylesheet/)<br>by HTML5 Doctor|[`normalize.css`](https://github.com/csstools/normalize.css)|[`sanitize.css`](https://github.com/csstools/sanitize.css/)|
|-|-|-|
|Підчищає будь-які стилі браузера|Приводить стилі різних бразерів до спільного знаменника|`normalize.css` + деякі штуки, які найчастіше доводиться писати|

Не використовуйте `reset.css`, ресетьте **тільки** те,
що можете й будете переписувати самі.
Ресетити все небезпечно,
бо легко недописавши чогось робите сайт менш доступним.

Використовуйте або `normalize.css`, або `sanitize.css`.
Додавайте свій ресет в проєкт тільки для тих частин,
які будете переписувати.
Можна робити покомпонентні ресети.


Як стилізувати інтерактивні елементи
-

### Кастомний checkbox чи радіо-кнопка

Додайте `appearance: none`,
але не забудьте стилізувати при цьому `:checked`, `:focus`, `:hover`, `:active`

### Іконки на `<input>` чи `<select>`

Додайте `background-image` та збільште `padding-inline-*` з відповідної сторони.

### Кнопка на `<input type=file>`

Використовуйте [`::file-selector-button`](https://developer.mozilla.org/docs/Web/CSS/::file-selector-button).

### `<input type=range>`

Дивіться [статтю на CSS Tricks](https://css-tricks.com/styling-cross-browser-compatible-range-inputs-css/)


Корисні ресурси
-

- [Ahmad Shadeed's Blog](https://ishadeed.com)
- [Every Layout](https://every-layout.dev)
- [CSS Layout Cookbook](https://developer.mozilla.org/docs/Web/CSS/Layout_cookbook)
