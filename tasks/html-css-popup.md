[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Telegram][icon-chat]][chat]

# HTML & CSS practice: Hooli-style Popup

> **Hooli** is a fictitious corporation from
> [Silicon Valley TV series](https://www.imdb.com/title/tt2575988/).
> Many believe it impersonates Google or Apple.
> Hooli on [Silicon Valley famdom wiki](https://silicon-valley.fandom.com/wiki/Hooli). 
> It is also represented [on the web](http://www.hooli.xyz/).
  
The goal of this task is to practice coding HTML & CSS from mockup. You are expected to deepen your knowledge of HTML & CSS and discover new previously unknown features.

## Requirements
- no JavaScript, only HTML/CSS, use of preprocessors is allowed
- no external libraries or frameworks
- browser support: Chrome only (feel free to use latest features)
- the popup is expected to have three states depending on user actions:
  - initial state: popup menu is not visible
  - upon click on ![popup-button](../img/popup-button.png) button 
    the popup menu gets visible or gets hidden if already open 
  - click on "More" button adds 3 to 10 more icons and 
    makes the content of the popup scrollable
- mobile view is irrelevant for this task

## Recommendations
- Make sure that your navigation is built by this structure: 
``` HTML
  <nav>
    <ul>
      <li>
        <a href='#'>Link</a>
      </li>
    <ul>
  </nav>
```
- Make sure that you've used visually-hidden for hiding inputs:
``` CSS
.visually-hidden {
	position: absolute !important;
	clip: rect(1px 1px 1px 1px); /* IE6, IE7 */
	clip: rect(1px, 1px, 1px, 1px);
	padding:0 !important;
	border:0 !important;
	height: 1px !important; 
	width: 1px !important; 
	overflow: hidden;
}
```
More info [here](https://htmlacademy.ru/blog/boost/frontend/short-12)
- Try to style your elements by classes (not by ID).
- Don't forget to set the `alt` attribute for the `img` tags (if you used them).
- No need to add a lot of files (inc. icons, gitignore, configs, etc) to your PR. HTML and CSS files would be enough for checking your work.
- Avoid external scripts for the font icons.
- Check your preview in the [validator](https://validator.w3.org/).
- Make sure you've added empty lines in each file from your PR.
- Check your code again and remove all redundant comments from your code.


## Warning

:warning: ![Google-Warning](https://place-hold.it/380x24/fff/f03c15?text=Important!+Google+may+ban+your+github+pages+domain!&bold)

The above may happen if your design mimics Google components or services
as they may decide that you've created a phishing site to steal
your visitors' Google credentials.

To avoid this
- DO NOT use word "google", "apple", "amazon" or any other brand in
  - your project/repo name
  - any urls
  - any css selectors
  - any HTML elements ids (including created with JS) or elsewhere across HTML
- DO NOT replicate Google design (layout structure, styles etc)
- DO NOT use Google icons

## Examples

You do not need to make your design 100% identical to the examples below.
Implementation of the mechanics is more important.
Use examples for your reference.

Initial state: no pop-up visible:

![popup-hidden](../img/popup-hidden.png)

Active state:

![popup-visible](../img/popup-visible.png)

Expanded set of icons, scrollable state:

![popup-scrollable](../img/popup-scrollable.png)

All interactive elements should be marked as such on mouse hover.

![popup-hover-state](../img/popup-hover.png)

All interactive elements should have `:focus` state.

![popup-hover-state](../img/popup-focus.png)

You'll must able to switch across all interactive elements using only keyboard(without a mouse, don't forget about styles for `:focus` state)

Feel free using [our icons](https://github.com/kottans/frontend/raw/master/img/popup-icons.zip).

You may want to publish your results on
[GitHub Pages](https://help.github.com/articles/configuring-a-publishing-source-for-github-pages/)

**When complete do the following:**
1. You will require code review for this task:
   - For **Frontend 2021** course students: please, follow [these instructions](https://github.com/kottans/frontend-2021-homeworks/blob/master/README.md)
   - For **p2p course** students: please, follow [these instructions](https://github.com/kottans/frontend-2019-p2p/blob/master/CONTRIBUTING.md)
1. Great job! Go ahead and share your progress with others –
   post a message in [course channel][chat]:
   `HTML-CSS-Popup — #done` (or `HTML-CSS-Popup — #p2p_done` if you are p2p course student) and add the link to your repo. **This step is important, as it helps mentors to track your progress!**

## Done?

➡️ Go forward to [JavaScript Basics](js-basics.md)

⤴️ Back to [Contents](../contents.md)


[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg

[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome#front-end-development
[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q
