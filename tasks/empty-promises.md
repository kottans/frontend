# Empty promises

This tasks will help you to understand `Promise` better. 

For this, you will need to create part of existing functionality of promises, like `Promise.all`, `Promise.race` and create [polyfills](https://remysharp.com/2010/10/08/what-is-a-polyfill) for functionality which don't exist right now, like `Promise.allSettled`.

## Existing functionality

You should remember, that you can override existing methods of `Promise` class and this called [monkey patching](https://en.wikipedia.org/wiki/Monkey_patch). But don't do this, because your code can brake `Promise` itself. Instead, you should expand functionality of `Promise`. For this, you should create some entity, which will extend it and then create your own methods on this extended entity.

For this, you can create your own class, which will extend `Promise`. Or you can use [Reflect.construct](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Reflect/construct).

1. Implement [Promise.all](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/all)
1. Implement [Promise.race](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/race)

## Polyfills

Note, that in this part you will create a polyfill. This means, that unlike previous task, you should add new methods to existing `Promise` and to some extended entity. But take into action, that when browser will have, saying `Promise.any`, your pollyfill should not be applied to `Promise`. So, add proper check. What check - figure out yourself. As an example, you can look to [Element.closest](https://developer.mozilla.org/en-US/docs/Web/API/Element/closest) polyfill.

1. Implement polyfill for [Promise.allSettled](https://github.com/tc39/proposal-promise-allSettled)
1. Implement polyfill for [Promise.any](https://github.com/tc39/proposal-promise-any)

## For brave one

Some time ago, our community had a proposal for cancelable promise. But because of evil guys from Google author closed [it](https://github.com/tc39/proposal-cancelable-promises). But we need a possibility to [cancel the promise](https://medium.com/@benlesh/promise-cancellation-is-dead-long-live-promise-cancellation-c6601f1f5082).

So you will, with help of the product of evil guys mentioned above, which is quite ironic I say, find a way how to create your own cancelable promise. In such a way you will restore justice in a galaxy.

Your promise must extend existing promise, of course.

1. Implement cancellable `Promise`