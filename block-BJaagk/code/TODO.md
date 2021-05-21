1. Convert the function below into different forms of function expression.

```js
// 1
function percentage(marks, total) {
  return (marks * 100) / total;
}
// 2
(function (marks, total) {
  return (marks * 100) / total;
})(50, 100);

// 3
percentage((marks, total) => {
  return (marks * 100) / total;
});
percentage(50, 100);

// Your code goes here
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
percentage(20, 100);
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
```

```js
let percentage = (marks, total) => (marks * 100) / total;
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.

4. Why is a function call an expression in JavaScript?

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Answer
five = add; // Answer
five = five(10, 11); // Answer
five = function () {
  return "Hello";
}; // Answer
```

6. What is the difference between function definition and function call? Explain with an example.

7. What is the similarities between function definition and function call?
<!-- Function defination contains the logic, while call contains what its going to process -->

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log("Hello World!");
}

hello.user = "Sam"; // valid or invalid
// invalid, as hello is a function and not an object
```

9. What is higher order function explain with an example.
<!-- One that has a callback function -->
10. Explain what is callback function. Why you can pass a function inside a function?
<!-- A callback function is a function that can be used for different purposes. Its passed inside a function -->
