---
title: Await in JavaScript
tags: function
cover: blog_images/image.jpg
firstSeen: 2023-01-18T05:00:00-04:00
---

In JavaScript, `await` is a keyword that can be used inside an `async` function to pause the execution of the function until a promise is resolved. It allows for synchronous-like code flow when working with asynchronous operations, such as API calls or reading from a file. The `await` keyword is used in front of an expression that returns a promise, and the resolved value of that promise is assigned to a variable.

JavaScript
```
async function example() {
  const response = await fetch('https://api.example.com');
  const data = await response.json();
  console.log(data);
}
```
In this example, the `fetch()` function returns a promise that resolves with a response object. The await keyword is used to pause the execution of the function until the promise is resolved, and the resolved value (the response object) is assigned to the response variable. The same process happens with the `response.json()` function, which also returns a promise that resolves with the data from the API.
