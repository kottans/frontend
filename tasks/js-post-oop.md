[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Telegram][icon-chat]][chat]

# OOP exercise

Now you know a lot about JavaScript OOP. Remember that
tiny JS world? Time to use your new power.

## Assignment

1. Improve your tiny JS world model you forked from
   [here](https://github.com/OleksiyRudenko/a-tiny-JS-world).
   This time use your favourite JS OOP methods to keep
   your code DRY and SOLID.

   You don't need forking this time, work with the repo you've
   already got. Git keeps history for you.
   
   You will find [these materials](https://github.com/OleksiyRudenko/a-tiny-JS-world/blob/master/README.md#learn-on-your-own) helpful.

### Most common issues to address

- [ ] If peer classes (siblings) have same properties those must be generalized to their base (parent) class
- [ ] Classes for species that do not have hands by natural design, do not consequently have hands or any equivalent property
      and do not inherit such properties from any of the base/parent classes
- [ ] Class properties that are parts of an object's presentation string are listed/specified explicitly
      (i.e. `Object` methods `values`, `keys`, `entires` or constructions like `for (key in obj)` aren't used)
- [ ] Object's presentation string builder is a class method, not an independent function
- [ ] Class constructor is defined with named parameters
- [ ] A class doesn't assign or change property owned by any other class (defined in any other class)
- [ ] A child class shouldn't directly use an inherited property to build an object's presentation string
- [ ] The code is [OOP](https://www.freecodecamp.org/news/object-oriented-programming-concepts-21bb035f7260/), SOLID ([eng](https://medium.com/@cramirez92/s-o-l-i-d-the-first-5-priciples-of-object-oriented-design-with-javascript-790f6ac9b9fa), [rus](https://medium.com/webbdev/solid-4ffc018077da)) and [DRY](https://code.tutsplus.com/tutorials/3-key-software-principles-you-must-understand--net-25161) compliant
- [ ] Got stuck or anything is not really clear? Ask a question

### Code review and assignment finalization

When complete do the following:
1. You will require code review for this task:
   - For **Frontend 2021** course students: please, follow [these instructions](https://github.com/kottans/frontend-2021-homeworks/blob/master/README.md)
   - For **p2p course** students: please, follow [these instructions](https://github.com/kottans/frontend-2019-p2p/blob/master/CONTRIBUTING.md)
   - Note, that especially this task requires you to submit
   a single file (`index.js` **only**) to the
   `frontend-2021-homeworks` or `frontend-2019-p2p` repo for code review.
1. Great job! Go ahead and share your progress with others –
   post a message in [course channel][chat]:
   `OOP Exercise — #done` (or `OOP Exercise — #p2p_done` if you are p2p course student)
   and add the link to your repo. **This step is important, as it helps mentors to track your progress!**
1. Study Extra Materials below to improve your skills and
   read an article or two on OOP under the links in
   [this repo](https://github.com/OleksiyRudenko/a-tiny-JS-world/blob/master/README.md#learn-on-your-own)

You have completed OOP tasks section.
We shall appreciate your feedback on this section especially
if you're doing this course from Ukraine.
Please, grant us 10-15 minutes of your time and **complete**
**[this feedback form](https://goo.gl/forms/sU4LKB6Ib3f659XD2)**.

When you finish this task you can proceed to the next one.

## Extra Materials

[Fun Fun Function - Composition over Inhertance](https://www.youtube.com/watch?v=wfMtDGfHWpA)

## Done?

➡️ Go forward to [Offline Web Applications](app-design-offline.md)

⤴️ Back to [Contents](../contents.md)

[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg

[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome#front-end-development
[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q
