[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Telegram][icon-chat]][chat]

# Friends App

Create a tiny social friends' search page with users cards,
search, sorting and filtering of them by age, name
or whatever you want with [Random User API](https://randomuser.me) :)

## Example

This is an *example*. You should style your application like you want. 

Make it personal. Make it beautiful. Make it perfect and then be proud for what you did.

![image](https://i.imgur.com/5tcpqcY.png)

Complete the user stories below.

## As a user, I would like to

* see cards list of users on the page, cards may be pretty styled with user photo, name, age, phone number, maybe with some another user information which you would to see in user info card.
* searching by typing name in search input and see immediately filtering on the page
* sorting cards by name/age in A-Z/Z-A ways
* filtering friends by age, by name, whatever you want else options
* see fancy icons and cool design with shadows, gradients, yellow font on the blue background, etc. Usage of template absolutely acceptable

## If you feel that you can do a better job, you can

Note, that this is an additional part of the task. Also you can implement anything from the list below.

### Be like a Durov and

* add pagination to scrolling
* sort not only by name and age, but also by date of registration
* filter by location and email
* make good responsive/fluid/elastic/whatever design which will work for mobiles
* use async/awaits for handling async actions

### Be like a Zuckerberg and

* add support of address bar which means, that user must see a state of filters and sortings in URL
* using your OOP knowledge, split your application to different parts, like: `FriendsList`, `FiltersContainer`, etc.
* with help of ES6 modules build website based on frontend components

## You can

- [ ] use all `Array.methods` which you know :) For instance - `Array#sort`,`Array#filter`, `Array#slice`, `Array#splice`, `Array#map`, `Array#reduce`, etc. Description of methods can be found [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
- [ ] try to figure out with async data encapsulation in request/response and try callbacks' logic in action
- [ ] understand sync/async `GET` requests, params & queries in action, something one of `fetch` or `XMLHttpRequest` but *NOT* jQuery. Because no ones like it ¯\_(ツ)_/¯
- [ ] understand pros & cons of the immutable fundamentals for complex types aka array on example of copies of arrays and how manage them
- [ ] you can try form' key/mouse events, manage them, enable and disable them

## Stuff which will help you

* We think that you will need to use promises for this task ;)
* [Основы XMLHttpRequest](https://learn.javascript.ru/ajax-xmlhttprequest) - you
  can use `XMLHttpRequest` for sending requests to webserver;
  [Method Fetch замена XHR](https://learn.javascript.ru/fetch) - you can use `fetch` as better tool for sending requests.
* [Randomuser api with awesome simple examples and docs](https://randomuser.me) -
  _you can use one of this API for getting data for your website_;
* [URL API](https://developer.mozilla.org/en-US/docs/Web/API/URL) - you can use
  this for working with URL;
* Take a look on [Array methods on learn.javascript.ru](https://learn.javascript.ru/array-methods)
* [Manipulating the browser history](https://developer.mozilla.org/en-US/docs/Web/API/History_API) -
  you must know how to work with browser history.

When you're done with your challenge push your code to GitHub repo and publish
it using [GitHub Pages](https://pages.github.com).

When complete do the following:
1. You will require code review for this task:
   * publish your task code base for review following instructions
     in [FE 2019 course homeworks repo](https://github.com/kottans/frontend-2019-homeworks)
   * when creating a PR do not forget to add a link
     to your app published on GitHub Pages
   * post links to your app on GitHub Pages and
     to your task PR in the
     [FE Questionarium chat](https://t.me/joinchat/DmX0JAl-mh5W0jrWli8Ycw)
     and ask mentors for a code review
   * once the code review phase successfully finished
     and you have an approval from one of the mentors
     add to your `kottans-frontend/README.md`
     the header `## Friends App`,
     a link to the app on GitHub Pages,
     a link to the task code base and
     a note saying `Reviewed and approved by @<mentor>`
     (use mentor's github username)
   * list your reflections on this task
     (_what was new to you_, _what surprised you_, _what you intend to use in future_)
1. You did a lot already! If you honestly finished all the previous steps then go ahead
   and share it with others –
   post a message in the [course channel][chat]:
   `Friends App — #done` and add the link to your repo. **This step is important, as it helps mentors to track your progress!**

## Done?

__Congratulations! 🎉__

* [ ] Have you finished all mandatory tasks?
* [ ] Are practical tasks get reviewed and
      PRs are merged into
      [frontend-2019-homeworks](https://github.com/kottans/frontend-2019-homeworks)
      repo `master`?

You have finished __Stage 0__ of the course!

Go ahead and post a celebration sticker or dancing gif
in the [course channel][chat].

... and a tiny thing to do yet.
[List yourself among course Stage 0 finishers](../students/stage0-finishers.md).

⤴️ Back to [Contents](../contents.md)


[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg

[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome#front-end-development
[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q
