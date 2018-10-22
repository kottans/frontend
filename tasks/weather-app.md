[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Telegram][icon-chat]][chat]

# Weather App

When you're done with your challenge push your code to github repo and publish
it using `gh-pages`. _Add link to it to your main frontend tasks repo._

If you honestly finished all the previous steps than go ahead and share it with
others - send a message in [course channel](chat) with the link to you repo and the words "Weather APP - finished" and add link to repo with code of the
website.

## Weather app

Create a page with a weather cast. As example, you can see forecast from
[darksky](https://darksky.net/forecast/50.4501,30.5241/us12/en).

### As a user, I would like to:

* enter the name of a city and get the forecast for it;
* see forecast for some period, not only for today. As example, for
  tomorrow, week, two weeks, etc;
* choose units — Celsius or Fahrenheit;
* have a list of favorite cities. By selecting favorite city from the list, I
  want to see forecast in it;
* have a list of recently viewed cities;
* see current city or latitude and longitude in the link in the address bar of
  the browser. If I open this link in the new window, website must show me
  weather in this city;
* see fancy icons for forecast and design. Usage of template absolutely
  acceptable.

You must support only last versions of major browsers — Chrome, Safari, FF,
Edge.

If you wish, you can support Internet Explorer, but this is not required. Same
story with mobile devices.

### Stuff which will help you:

* [Основы XMLHttpRequest](https://learn.javascript.ru/ajax-xmlhttprequest) - you
  can use XMLHttpRequest for sending requests to webserver;
* [Weather public API's](https://github.com/toddmotto/public-apis#weather) -
  _you can use one of this API for getting data for your website_;
* [URL API](https://developer.mozilla.org/en-US/docs/Web/API/URL) - you can use
  this for working with URL;
* [Manipulating the browser history](https://developer.mozilla.org/en-US/docs/Web/API/History_API) -
  you must know how to work with browser history.

### If you feel that you can do a better job, you can:

#### Choose path of master of sun and clouds, and:

* use
  [async/awaits](https://medium.freecodecamp.org/javascript-from-callbacks-to-async-await-1cc090ddad99)
  and [fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
  for handling network requests;
* with help of ES6 modules build website based on frontend components (aware,
  that FF do not support ES6 modules right now).
* make good responsive/fluid/elastic/whatever design and other modern stuff;

#### Choose path of grandmaster of storms, tornadoes for all over the time, space and in all possible far-far away, and:

* see video, which will give basic understanding about architecture of modern
  website —
  [Nicholas Zakas: Scalable JavaScript Application Architecture](https://www.youtube.com/watch?v=vXjVFPosQHw);
* after finishing above mentioned video, try to build your website from
  components. As example:

  - Application — fetching, storing and processing all the data
  - SearchBar — controls search input, sends input data to Application
  - TodayForecast — takes data from Application and shows forecast for today
  - WeekForecast — takes data from Application and shows forecast for week
  - TemperatureDropdown — dropdown, which gives possibility to select Celsius or
    Fahrenheit

### Additional information

* The exact list of forecast periods may depend on API which you choose for this
  task. Providing forecast not for week, but for five days, 10 days, etc.
  totally acceptable;
* In case you try to build modular frontend application, you can skip support
  of FF, because last one does not support ES6 modules;
* Map with temperatures is not required for this task;

## Done?

__Congratulations! 🎉__

You have finished __Stage 0__ of the course!

➡️ Go to [Course Chat][chat] and let us know about!

⤴️ Back to [Contents](../contents.md)


[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg

[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome#front-end-development
[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q
