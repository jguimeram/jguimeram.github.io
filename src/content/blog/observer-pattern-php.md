---
title: 'Observer pattern in PHP'
description: 'Building a concrete example of observers and subjects.'
pubDate: 'Jun 21 2024'
heroImage: '../../assets/blog-placeholder-4.jpg'
---
The observer pattern establishes a one-to-many relationship between objects so that when one object changes state, all of its dependents are notified. This is ideal for event-driven code where various components need to react to the same occurrence.

In PHP you might define a `Subject` interface with methods to attach, detach and notify observers. Individual observers implement an `update()` method and register with the subject to receive notifications. Whenever the subject's internal data changes, it calls `update()` on each observer.

A practical example is a blog system where publishing a new post triggers email notifications and cache invalidation. By relying on the observer pattern these behaviors are decoupled from the publishing code and can be added or removed with minimal changes.


