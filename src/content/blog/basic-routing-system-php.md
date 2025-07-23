---
title: 'Basic routing system in PHP'
description: 'Creating a lightweight routing layer for handling HTTP requests.'
pubDate: 'Jun 22 2024'
heroImage: '../../assets/blog-placeholder-5.jpg'
---

A routing system maps incoming URLs to code that should handle the request. While full frameworks provide sophisticated routers, you can craft a small version using plain PHP for learning purposes or lightweight projects.

One approach is to store routes in an associative array where keys represent URL patterns and values are anonymous functions or class methods. On each request you inspect the current path, look it up in the array and execute the corresponding callback.

By building a minimal router yourself you gain insight into how frameworks dispatch requests and you retain full control over what happens before and after each route is processed.
