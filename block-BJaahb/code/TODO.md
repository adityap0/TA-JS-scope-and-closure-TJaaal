Create the execution context diagram for the following code snippets:

```js
function outer() {
  let b = 10;
  function inner() {
    let a = 20;
    console.log(a + b);
  }
  return inner;
}
let getSum = outer();
let num = getSum();
```

<!-- Ans link -
https://excalidraw.com/#json=6105212800466944,bZlOut8HcAwPdlvlRzsmmw -->

2.

Create the execution context diagram for following code. Also write the output of the code below.

```js
function getCounter() {
  let count = 0;

  return () => {
    return count++;
  };
}

let counter = getCounter();

counter(); // output
counter(); // output
counter(); // output
counter(); // output
```

<!-- https://excalidraw.com/#json=5542262847045632,oaNhEa0LAY35O6z2qhnR6A -->

3. Create the execution context diagram

```js
function makeColorChanger(color) {
  return function () {
    document.body.style.backgroundColor = color;
  };
}

let blue = makeColorChanger("blue");
let tomato = makeColorChanger("tomato");

blue();
tomato();

// https://excalidraw.com/#json=6205062200164352,9u5fhHBi5uJLPOzuztYC8g
// What will be the background color after the execution of last line = tomato
```
