[![MIT Licensed][icon-mit]][license]
[![Ideas and useful links][icon-ideas]][ideas]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Telegram][icon-chat]][chat]

# Task 13

Pizza App: API, auth, routing

### Login And Registration
Our future pizza management service needs to know which manager performing some actions. Using experience gained from Task 10,
we are going to create a part of single page application with simple authorization flow.

#### Key Terms
- router
- component
- authentication
- authorization
- JWT

#### Task Description

- Create Native JavaScript router using [history API](https://developer.mozilla.org/en-US/docs/Web/API/History)
or [hash-changed](https://developer.mozilla.org/ru/docs/Web/Events/hashchange) browser event. [Example](https://github.com/zonzujiro/spa-framework/blob/master/src/framework/Router.js).
- Transform your pizza dashboard page from Task 12 into [component](https://github.com/zonzujiro/spa-framework/blob/master/src/framework/Component.js).
- Add two or two-in-one pages to your app - Registration and Login.
- Using [Kottans Pizza API](https://github.com/lempiy/Kottans-Pizza-Api) implement registration and login functionality on your authorization pages.

*IMPORTANT. In order to register new user in the system you will need to have your own "pizza store"
bound to your application. To pick one, type private message on Gitter to **@lempiy** with store name and store password
you want to use.*

- Secure your dashboard page from Task 12 with authorization permission - non-authorized
users should be redirected to login page.
- Create user profile page that should be also secured with authorization permission. Use the data from [my_info](https://github.com/lempiy/Kottans-Pizza-Api/blob/master/docs/USERS.md#my-info) API method.
- As always, feel free to ask your questions in our chat.

#### GOOD LUCK!

#### Resources

- [A modern JavaScript router in 100 lines](http://krasimirtsonev.com/blog/article/A-modern-JavaScript-router-in-100-lines-history-api-pushState-hash-url)
- [Cookies vs Tokens: The Definitive Guide](https://auth0.com/blog/cookies-vs-tokens-definitive-guide/)
- [Про токены, JSON Web Tokens (JWT), аутентификацию и авторизацию](https://gist.github.com/zmts/802dc9c3510d79fd40f9dc38a12bccfc)
- [Native JS SPA Example](https://github.com/zonzujiro/spa-framework)


[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg

[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome#front-end-development
[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q
