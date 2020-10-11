[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Telegram][icon-chat]][chat]

# Weather App

When you're done with your challenge push your code to github repo and publish
it using `gh-pages`. _Add link to it to your main frontend tasks repo._

Great job! Go ahead and share your progress with others - send a message in [course channel](chat) with the link to you repo and the words "Weather APP - finished" and add link to repo with code of the
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
* Map with temperatures is not required for this task;

#### Video

You can see workshop's screencast below.

|||    
--- | --- 
[![WebApp - Design Patterns - Oleksiy Rudenko][first-ws-img]][first-ws] | [WebApp - Design Patterns - Oleksiy Rudenko][first-ws]
[![Weather App (p.1) - Oleksiy Rudenko][second-ws-img]][second-ws] | [Weather App (p.1) - Oleksiy Rudenko][second-ws]
[![Weather App (p.1 continued) - Oleksiy Rudenko][third-ws-img]][third-ws]|[Weather App (p.1 continued) - Oleksiy Rudenko][third-ws]
[![Weather App (p.1 Retro) - Oleksiy Rudenko][fourth-ws-img]][fourth-ws]|[Weather App (p.1 Retro) - Oleksiy Rudenko][fourth-ws]
[![Weather App (p.2) State Management - Oleksiy Rudenko][fifth-ws-img]][fifth-ws]|[Weather App (p.2) State Management - Oleksiy Rudenko][fifth-ws]
[![Improving Component Rendering (p.1) - Oleksiy Rudenko][sixth-ws-img]][sixth-ws]|[Improving Component Rendering (p.1) - Oleksiy Rudenko][sixth-ws]
[![Improving Component Rendering (p.2) - Oleksiy Rudenko][seventh-ws-img]][seventh-ws]|[Improving Component Rendering (p.2) - Oleksiy Rudenko][seventh-ws]
[![Routing Intro - Christina Landvytovych][eighth-ws-img]][eighth-ws]|[Routing Intro - Christina Landvytovych][eighth-ws]
[![Routing Workshop - Mykhailo Hanol][ninth-ws-img]][ninth-ws]|[Routing Workshop - Mykhailo Hanol (1/3)][ninth-ws]
[![Routing Workshop - Mykhailo Hanol][tenth-ws-img]][tenth-ws]|[Routing Workshop - Mykhailo Hanol (2/3)][tenth-ws]
[![Routing Workshop - Mykhailo Hanol][eleventh-ws-img]][eleventh-ws]|[Routing Workshop - Mykhailo Hanol (3/3)][eleventh-ws]

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

[first-ws]: https://youtu.be/NQ6xHcQuQe4
[first-ws-img]: http://img.youtube.com/vi/NQ6xHcQuQe4/default.jpg
[second-ws]: https://youtu.be/FcPx2AC77DQ
[second-ws-img]: http://img.youtube.com/vi/FcPx2AC77DQ/default.jpg
[third-ws]: https://youtu.be/CSpnXeaBomE
[third-ws-img]: http://img.youtube.com/vi/CSpnXeaBomE/default.jpg
[fourth-ws]: https://youtu.be/o1L0DvcqmDU
[fourth-ws-img]: http://img.youtube.com/vi/o1L0DvcqmDU/default.jpg
[fifth-ws]: https://youtu.be/TC0ROTuYAlo
[fifth-ws-img]: http://img.youtube.com/vi/TC0ROTuYAlo/default.jpg
[sixth-ws]: https://youtu.be/EDzPXul5teA
[sixth-ws-img]: http://img.youtube.com/vi/EDzPXul5teA/default.jpg
[seventh-ws]: https://youtu.be/z9spriQGo5M
[seventh-ws-img]: http://img.youtube.com/vi/z9spriQGo5M/default.jpg
[eighth-ws]: https://youtu.be/UKjbmvl4WQU
[eighth-ws-img]: http://img.youtube.com/vi/UKjbmvl4WQU/default.jpg
[ninth-ws]: https://youtu.be/AVYPMZIdAIw
[ninth-ws-img]: http://img.youtube.com/vi/AVYPMZIdAIw/default.jpg
[tenth-ws]: https://youtu.be/JUTb6SY48-Y
[tenth-ws-img]: http://img.youtube.com/vi/JUTb6SY48-Y/default.jpg
[eleventh-ws]: https://youtu.be/VvbL9HEZpjY
[eleventh-ws-img]: http://img.youtube.com/vi/VvbL9HEZpjY/default.jpg
