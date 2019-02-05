# Empty promises

This tasks will help you to understand `Promise` better. 

For this, you will need to create part of existing functionality of promises, like `Promise.all`, `Promise.race` and create [polyfills](https://remysharp.com/2010/10/08/what-is-a-polyfill) for functionality which don't exist right now, like `Promise.allSettled`.

## It is a last candy...

**Existing functionality**

You should remember, that you can override existing methods of `Promise` class and this called [monkey patching](https://en.wikipedia.org/wiki/Monkey_patch). But don't do this, because your code can brake `Promise` itself. Instead, you should expand functionality of `Promise`. For this, you should create some entity, which will extend it and then create your own methods on this extended entity.

For this, you can create your own class, which will extend `Promise`. Or you can use [Reflect.construct](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Reflect/construct).

1. Implement [Promise.all](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/all)
1. Implement [Promise.race](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/race)

## Last episode and I go to bed...

**Polyfills**

Note, that in this part you will create a polyfill. This means, that unlike previous task, you should add new methods to existing `Promise` and to some extended entity. But take into action, that when browser will have, saying `Promise.any`, your pollyfill should not be applied to `Promise`. So, add proper check. What check - figure out yourself. As an example, you can look to [Element.closest](https://developer.mozilla.org/en-US/docs/Web/API/Element/closest) polyfill.

1. Implement polyfill for [Promise.allSettled](https://github.com/tc39/proposal-promise-allSettled)
1. Implement polyfill for [Promise.any](https://github.com/tc39/proposal-promise-any)

## I will start from Monday...

**Missing functionality. Part 1. For brave one**

What if you need to cancel a promise? Saying, you have sent a network request, you haven't received a result and the user leaves the page. You don't need a result of this request and a server can stop working on it, right?

Some time ago, our community had a proposal for cancelable promise. But because of evil guys from Google author closed [it](https://github.com/tc39/proposal-cancelable-promises). But we need a possibility to [cancel the promise](https://medium.com/@benlesh/promise-cancellation-is-dead-long-live-promise-cancellation-c6601f1f5082).

So you will, with help of the product of evil guys mentioned above, which is quite ironic I say, find a way how to create your own cancelable promise. In such a way you will restore justice in a galaxy.

Your promise must extend existing promise, of course.

1. Implement cancellable `Promise`

**Missing functionality. Part 2.**

You know, how `Promise.all` works, right? It will launch all asynchronous functions simultaneously.

But what we can do, if we need to run several functions one-by-one? :thinking: `Promise.chain` will help us! This method should receive as an argument array of promises and then call them one by one (you see why "chain" right?) and return result.

Little tip: `Array#reduce`

1. Implement `Promise.chain`


## When complete do the following:
1. You will require code review for this task:
   - If you are a **p2p course** student, please, follow [these instructions](https://github.com/kottans/frontend-2019-p2p/blob/master/CONTRIBUTING.md)
   - If you are a student of the **offline** Kottans course, please, follow [these instructions](https://github.com/kottans/frontend-2019-homeworks/blob/master/README.md)
1. You did a lot already! If you honestly finished all the previous steps then go ahead
   and share it with others –
   post a message in the [course channel][chat]:
   `Empty promises — #done` (or `Empty promises — #p2p_done` if you are p2p course student) and add the link to your repo. **This step is important, as it helps mentors to track your progress!**

When you finish this task you can proceed to the next one.
