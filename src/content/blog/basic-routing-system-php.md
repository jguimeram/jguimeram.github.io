---
title: 'Basic routing system in PHP'
description: 'Creating a lightweight routing layer for handling HTTP requests.'
pubDate: 'Jun 22 2024'
heroImage: '../../assets/blog-placeholder-5.jpg'
---

Learn how to set up a minimal routing system in PHP using associative arrays and anonymous functions to map URLs to handlers.

A routing system maps incoming URLs to code that should handle the request. While full frameworks provide sophisticated routers, you can craft a small version yourself.

One approach is to store routes in an associative array where keys represent URL patterns and values are anonymous functions or class methods. On each request, your router matches the path to a handler.

By building a minimal router yourself you gain insight into how frameworks dispatch requests and you retain full control over what happens before and after each route executes.

