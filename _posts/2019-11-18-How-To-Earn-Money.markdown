---
title: How To Earn Money
layout: post
tags: technologies
---

**Asynchronous **programming is very common in the Javascript world because of the event-driven nature of tasks. One of the most common pattern used is that of the callbacks (Continuation-passing style paradigm). People (including myself) prefer using the async/await pattern instead. JS now has in-built support for async/await and the most common libraries often provide both the interfaces (async/await and callbacks). A lot of older libraries have not moved on though. For such libraries, it is possible to wrap the functionality in a Promise to provide a thenable interface (works with async/await).

Things are slightly more complicated on the Typescript front though. Ideally, we want complete type-safety without adding anything extra from our side. It is possible to achieve this in Typescript. The most important thing is for this is to somehow extract the argument type of the callback function and assign it to the T variable in Promise<T> interface.

[iamsushanth.github.io](http://iamsushanth.github.io)