# forEach

[`forEach`][forEach-helper] is an array helper method. We have access to `forEach` method on any given array. We pass in an anonymous function to the `forEach` helper which gets called one time for every element in the array and whatever is inside the function would be executed.

```js
let colors = [ 'red', 'green', 'blue' ];

colors.forEach((color) => {
  console.log(color);
});

// red
// green
// blue
```

```js

// 'colors' array                                  result array

// red
// green ---------> Iterator Function ---------> do something
// blue

// (the Iterator Function gets called one time for every element in the array and returns then goes to the next element if there are any left)

```

---

### Example(s)

```js
let numbers = [1, 2, 3, 4, 5];

let sum = 0;

number.forEach((number) => {
  sum += number;
});

// 15
```


[forEach-helper]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach
