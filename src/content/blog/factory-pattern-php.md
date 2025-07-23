---
title: 'Factory pattern in PHP'
description: 'How to decouple object creation using a simple factory class.'
pubDate: 'Jun 20 2024'
heroImage: '../../assets/blog-placeholder-3.jpg'
---

The factory pattern provides a single point for creating objects, making it easier to change which classes are instantiated without touching the code that uses them. A factory can examine input or configuration and return the appropriate object type.

In PHP, a basic factory class exposes a method like `create()` that returns different implementations of an interface. This keeps the client code agnostic about the specific classes being created and lets you manage dependencies in one place.

Below is a short example of a vehicle factory. Depending on a given type, the factory returns either a `Car` or a `Truck` object. This pattern simplifies object management and improves maintainability as your application grows.
