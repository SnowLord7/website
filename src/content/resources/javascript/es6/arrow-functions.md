---
authors:
  - "veksen#1060"
  - "Drew Snow#1286"
title: "Arrow functions"
created_at: 2019/10/08
updated_at: 2019/10/09
external_resources:
  - "https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions"
  - "https://www.sitepoint.com/es6-arrow-functions-new-fat-concise-syntax-javascript/"
  - "https://exploringjs.com/es6/ch_arrow-functions.html"
---

## Intro to Arrow Functions

An arrow function in Javascript is a shorter version of the normal function syntax. In general you may not notice much of a difference between the two, however there are some small yet important differences.

## Normal Functions:

Normal function may look similar to the following:

```js
const foo = function () {
  return 'bar';
}
```

## Arrow Functions

Arrow functions are typically used to simplify code, or make it easier to read. A typical arrow function may look like to following:

```js
const foo = () => {
  return 'bar';
}
```

## Arrow Functions Return Default

If the arrow function only has one statement, and the statement is the return value, you can simplify the function even more.

```js
const foo = () => 'bar';
```

## Arrow Functions and Parameters

Arrow functions support parameters similar to normal functions, however if there is only one parameter you are able to remove the parentheses.

Arrow function with only one parameter:
```js
const foo = bar => 'baz';
```

Arrow function with multiple parameters:
```js
const foo = (bar, baz) => 'qux';
```

## Differences with Arrow Functions

When working with arrow functions you might notice that the `this` keyword is not available in the arrow function. The `this` keyword will always represents the object that defined the arrow function.
