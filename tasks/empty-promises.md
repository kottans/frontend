# Empty promises

This tasks will help you understand `Promise` better.

You're gonna create a part of promises' existing functionality, like `Promise.all`, `Promise.race` and create [polyfills](https://remysharp.com/2010/10/08/what-is-a-polyfill) for functionality which doesn't exist yet, like `Promise.allSettled`.

## Last piece of candy...

**Existing functionality**

You should remember that you can override existing methods of `Promise` class — this is called [monkey patching](https://en.wikipedia.org/wiki/Monkey_patch). However, don't do this, because your code can break `Promise` itself. Instead, you should expand functionality of `Promise`. For this, you should create some entity, which will extend it and then create your own methods on this extended entity.

For example, you can create your own class which will extend `Promise`, or you can use [Reflect.construct](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Reflect/construct).

1. Implement [Promise.all](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/all)
1. Implement [Promise.race](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/race)

## Last episode before bed...

**Polyfills**

In this part you will create a polyfill. This means that, unlike previous task, you should add new methods to existing `Promise` and to some extended entity. But take into account that, when the browser will have, say, `Promise.any`, your polyfill should not be applied to `Promise`. So, add a proper check. What check - figure out yourself. As an example, you can look at [Element.closest](https://developer.mozilla.org/en-US/docs/Web/API/Element/closest) polyfill.

1. Implement polyfill for [Promise.allSettled](https://github.com/tc39/proposal-promise-allSettled)
1. Implement polyfill for [Promise.any](https://github.com/tc39/proposal-promise-any)

## I will start from Monday...

**Missing functionality. Part 1. For the brave one**

What if you need to cancel a promise? Say, the server has received a network request, started working on the result, but before it could send it back the user has already left the page. You don't need a result of this request and a server can stop working on it, right?

Some time ago, our community had a proposal for cancelable promise. But because of evil guys from Google author closed [it](https://github.com/tc39/proposal-cancelable-promises). But we need a possibility to [cancel the promise](https://medium.com/@benlesh/promise-cancellation-is-dead-long-live-promise-cancellation-c6601f1f5082).

So you will, with help of the product of evil guys mentioned above, which is quite ironic I say, find a way how to create your own cancelable promise. In such a way you will restore justice in a galaxy.

Your promise must extend existing promise, of course.

1. Implement cancellable `Promise`

**Missing functionality. Part 2.**

You know, how `Promise.all` works, right? It will launch all asynchronous functions simultaneously.

But what if we need to run several functions one-by-one? 🤔 `Promise.chain` will help us! This method should receive as the argument an array of promises and then call them one by one and return the result.

Little tip: `Array#reduce`

1. Implement `Promise.chain`

## When complete do the following:

1. You will require code review for this task:
   - For **Frontend 2021** course students: please, follow [these instructions](https://github.com/kottans/frontend-2021-homeworks/blob/master/README.md)
   - For **p2p course** students: please, follow [these instructions](https://github.com/kottans/frontend-2019-p2p/blob/master/CONTRIBUTING.md)
1. Great job! Go ahead
   and share your progress with others –
   post a message in the [course channel][chat]:
   `Empty promises — #done` (or `Empty promises — #p2p_done` if you are p2p course student) and add the link to your repo. **This step is important, as it helps mentors to track your progress!**

When you finish this task you can proceed to the next one.

[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q