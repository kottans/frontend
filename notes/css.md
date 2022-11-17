Основи CSS
==========

Cascading and Inheritance
-

### Специфічність

Селектори за зростом специфічності:
- `type`
- `.class`, `[attribute]`
- `#id`
- inline `style="..."`

Якщо вдаватися в деталі, специфічність — це число,
де частини нижчого рангу представляють нижчі порядки:
```
[ inline ][ id ][ class/attribute/pseudo-class ][ type/pseudo-element ]
```

Наприклад, для селектора
`span.visually.hidden:not(:focus, :focus-within)` —
`[0][0][3][1] = 31` (`:not()` має специфічніть того, що всередині).

### !important

Властивості позначені `!important` кладуться в **окрему** пріоритетну чергу.

Специфічніть в пріоритетній черзі поміж елементами визначається таким же чином, але всі _важливі_ властивості будуть мати вищу специфічність, ніж будь-який селектор в нормальній черзі.


### `:is()`, `:where()` — комбінованi селектор

Дозволяє комбінувати довгі селектори зручніше.
Для `:is()` специфічність рахується так само, ніби вони були розвернуті без `:is()`.

Наприклад, селектор довільної секції, яка йде зразу після довільної секції:

```css
:is(article, aside, section, nav) + :is(article, aside, section, nav) {
	margin-block-start: 1rem;
}
```

Це аналогічно до перебору усіх комбінацій:
```css
article + article,
article + aside,
article + section,
article + nav,

aside + article,
/* ... 11 селекторів опущено */
nav + nav {
	margin-block-start: 1rem;
}
```

`:where()` працює аналогічно, але має специфічність 0.


### `:has()`

Дозволяє стилізувати елемент, який має певні дочірні або сусідні елементи, які відповідають селектору всередині.

`article:has(h2)` — це така стаття, всередині якої є заголовок другого рівня.


### Псевдо-елементи

`::before` та `::after` для того, щоб можна було дадавати _презентаційний_ контент елементам —
такий, що не несе смислового навантаження, ні візуального, ні текстового.
Якщо без контенту в них не можна обійтися, або треба, щоб він копіювався,
цей контент має бути в розмітці, а не в стилях.

`::before` та `::after` не можна виділити чи скопіювати, їх немає в [replaced elements](https://developer.mozilla.org/docs/Web/CSS/Replaced_element) (`img`, `input`); вони додаються тільки коли є `content`, і стандартно мають `display: inline`.

Інші псевдо-елементи додволяють стилізувати те, чого явно немає в дереві документу —
виділення (`::selection`),
маркери списків (`::marker`),
текст-підказка (`::placeholder`),
першу літеру чи рядок (`::first-letter`, `::first-line`).

[Список псевдо-елементів на MDN](https://developer.mozilla.org/docs/Web/CSS/Pseudo-elements)

### Псевдо-класи

Для того, щоб можна було доступитися до специфісних станів елементів, наприклад, `:visited`, `:invalid`.

[Список псевдо-класів на MDN](https://developer.mozilla.org/docs/Web/CSS/Pseudo-classes)


Values and Units
-
Використовуйте `rem` та `em` для віступів та полів (`margin`, `padding`, `gap` тощо).
Використовуйте ці та інші відносні до розміру шрифту величини — `ch`, `lh`, `ex`, `cap`, а також відсотки (`%`) для встановлення розмірів елементів, де це необхідно.
Це робить дизайн гнучким до налаштувань шрифту **користувача**.

Використовуйте <b>новий синтаксис</b> для написання кольорів:
```
Старий:
rgba(r, g, b)
rgb(r, g, b)

Новий:
rgb(r g b / a)
hsl(h s l / a)
```

Генерувати кольорові схеми <mark>з логічною градацією світності</mark> найзручніше в просторах LAB та OKLAB:
```
lch(lighness chroma hue / alpha)
oklch(lighness chroma hue / alpha)
```

Список на [MDN](https://developer.mozilla.org/docs/Learn/CSS/Building_blocks/Values_and_units)
Специфікація про кольори: [CSS Color Module Level 4](https://www.w3.org/TR/css-color-4/)


Box Model
-

![CSS Box Model](https://www.w3.org/TR/css-box-4/images/box.png)

Специфікація: [CSS Box Model Level 4](https://www.w3.org/TR/css-box-4/)


### Display

<b>Відображення</b> елемента є:
- <b>зовнішнє</b>&nbsp;— те, як він веде себе в просторі батькіського елемента; та
- <b>внутрішнє</b>&nbsp;— те, яке середовище він створює для дочірніх елементів.

Специфікація: [CSS Display Level 3](https://www.w3.org/TR/css-display-3/#the-display-properties)


Writing Modes
-

Різні мови записуються по-різному.
Наприклад, японська зазвичай пишеться зверху вниз та справа наліво.
Для роботи з цим є `writing-mode`, який має наступні значення:

|horizontal-tb|vertical-rl|vertical-lr|
|-|-|-|
|![horizontal](https://www.w3.org/TR/css-writing-modes-3/images/horizontal.png)|![vertical right to left](https://www.w3.org/TR/css-writing-modes-3/images/vertical-rl.png)|![vertical left to right](https://www.w3.org/TR/css-writing-modes-3/images/vertical-lr.png)|
|горизонтальний<!--, або зліва направо, або справа наліво, або в обидві сторони; зверху вниз-->|вертикальний спрва наліво|вертикальний зліва направо|

Різні методи письма може й не знадобляться для того,щоб працювати з різними мовами, але необхідні для розуміння логічних властивотей для розміру та полів 👇

Специфікація: [CSS Writing Modes Level 3](https://www.w3.org/TR/css-writing-modes-3/)


Physical & Logical Properties
-

Фізичні відповідають сторонам пристрою. Логічні відповідають методу написання.
Застосовуються для `margin`, `padding`, `border`, `border-radius`, позиціонування та розмірів.

Використовуте ті, які вам потрібні в контексті.
Якщо це відступ між абзацами, то це логічний відступ.
Якщо це поля контейнера, то це або фізичний, або логічний відступ.

Приклад для `margin`:

|Фізичні|Логічні для англійської/української|
|-|-|
|margin-top|margin-block-start|
|margin-bottom|margin-block-end|
|margin-left|margin-inline-start|
|margin-right|margin-inline-end|

Специфікація: [CSS Logical Properties and Values Level 1](https://www.w3.org/TR/css-logical-1/)


Organizing CSS & Naming Conventions
-

### Component-* vs utility-based class names

-	BEM — суто компонентний підхід
-	ACSS (Tailwind) суто утилітний підхід

Недоцільно мати утиліти, які буквально повторюють одну CSS-властивість із заданим значенням, як от `pb-4`.
Так само недоцільно для кожного компонента повторювати, що в нього повинні бути заокруглені кути, білий фон і сіра рамка.
Краще бути десь посередині. Наприклад:

```css
.box {
	padding: 1rem;
	border: 1px solid #eee;
	border-radius: .25rem;
	background-color: #fff;
}
```

#### [Інші методи організації CSS](https://clubmate.fi/oocss-acss-bem-smacss-what-are-they-what-should-i-use)
-	Atomic Design
-	OOCSS
-	SMACSS

### Як сортувати поля всередині селекторів

Найпопулярніша методологія запозичена з [recess](https://github.com/stormwarning/stylelint-config-recess-order/blob/main/index.js):
- позиція
- дисплей
- флекси/ґріди
- розміри й поля
- шрифти й текст
- рамки й фони
- анімації

Якщо використовувати [Stylelint](http://stylelint.io), то трохи легше.

Pre-processors & Post-processors
-

Препроцесори генерують із мета-CSS — CSS.
Постпроцесори (процесори) перетворюють CSS в CSS.

Коли вам необхідно геренувати із мета-коду CSS, використовуйте препроцесор.
В усіх інших випадках їх використання не є доцільним.
CSS-процесор доцільно використовувати, коли хочеться писати сучасний CSS,
мати чистий код і при цьому підтримувати старіші браузери.

Приклад для препроцесора — генерація [типографічної шкали](https://spencermortensen.com/articles/typographic-scale/):
- [бібліотека функцій](https://github.com/viktor-yakubiv/css/blob/a8dcfd15c3929f8d1d40b0da88c7baac351c3bea/lib/_scale.scss)
- [генератор](https://github.com/viktor-yakubiv/css/blob/a8dcfd15c3929f8d1d40b0da88c7baac351c3bea/scale.scss)
- [результат](https://github.com/viktor-yakubiv/css/blob/a8dcfd15c3929f8d1d40b0da88c7baac351c3bea/scale.css)

Приклад для процесора — [перетворення кольорів](https://github.com/viktor-yakubiv/css/blob/a8dcfd15c3929f8d1d40b0da88c7baac351c3bea/color.css) з новго синтаксису й простору у старіший,
щоб підтримувати ширший спектр браузерів.


### Пре-процесори

На сьогодні активний — [SASS](https://sass-lang.com).

До речі, про nesting, не використовуйте. Це прикольно, але без нього легше.
Чим ближче ви до стандарту, тим зрозуміліший код.

### (Пост)процесори

[PostCSS](https://postcss.org)

- [preset-env](https://preset-env.cssdb.org/)
- [autoprefixer](https://autoprefixer.github.io)
- [browserslist](https://browserslist.dev/?q=bGFzdCAyIHZlcnNpb25z)
