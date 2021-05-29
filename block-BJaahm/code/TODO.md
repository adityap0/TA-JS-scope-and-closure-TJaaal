1. Construct a function intersection that compares input arrays and returns a new array with elements found in all of the inputs. You can only use reduce method to do this.

```js
function intersection(...arrays) {
  let finalArr = arrays[0].reduce((acc, cv) => {
    let count = 0;
    for (i = 1; i < arrays.length; i++) {
      if (arrays[i].includes(cv)) {
        count += 1;
      }
    }
    if (count === arrays.length - 1) {
      acc.push(cv);
    }
    return acc;
  }, []);
  return finalArr;
}

// Test
console.log(
  intersection([5, 10, 15, 20], [15, 88, 1, 5, 7], [1, 10, 15, 5, 20])
); // should log: [5, 15]
```

2. Construct a function `union` that compares input arrays and returns a new array that contains all elements. If there are duplicate elements, only add it once to the new array. Preserve the order of the elements starting from the first element of the first input array. You can only use reduce method to do this.

```js
function union(...arrays) {
  let finalArr = [];
  let solution = [];
  arrays.forEach((innerArr) => {
    innerArr.forEach((item) => {
      finalArr.push(item);
    });
  });
  finalArr.forEach((item, i) => {
    if (i === finalArr.indexOf(item)) {
      solution.push(item);
    }
  });
  return solution;
}

// Test
console.log(union([5, 10, 15], [15, 88, 1, 5, 7], [100, 15, 10, 1, 5]));
// should log: [5, 10, 15, 88, 1, 7, 100]
```
