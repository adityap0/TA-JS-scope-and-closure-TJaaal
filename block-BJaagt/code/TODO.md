Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = "Arya";
}
console.log(useranme); // Error
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = "Arya";
}
console.log(useranme); // Error
```

In the above code the username is defined inside a block therefore it will show an erro

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = "Arya";
}
console.log(useranme); // Error
```

In the above code the username is defined inside a block therefore it will show an error.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = "Arya";
}
console.log(useranme); // error
```

In the above code the username is defined inside a block therefore it will show an error.

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = "John";
if (true) {
  var username = "Arya";
}
console.log(useranme); // Error, username defined twice
```

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = "John";
if (true) {
  let username = "Arya";
}
console.log(useranme); // Error, username defined twice
```

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = "John";
function sayHello() {
  let username = "Arya";
}
sayHello();
console.log(useranme); // Error, username defined twice
```

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, "First"); // (0...9) First
}
console.log(i, "Second"); // 10, Second
```

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, "First"); // same as above
}
console.log(i, "Second"); // same as above
```
