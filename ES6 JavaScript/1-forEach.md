# forEach

[`forEach`][forEach-helper] is and array helper method. We have access to `forEach` method on any given array. We pass in an anonymous function to the `forEach` helper which gets called one time for every element in the array and whatever is inside the function would be executed.

```js
let colors = [ 'red', 'green', 'blue' ];

colors.forEach((color) => {
  console.log(color);
});
```

output:
```js
// red
// green
// blue
```

### Example

```js
let numbers = [1, 2, 3, 4, 5];

let sum = 0;

number.forEach((number) => {
  sum += number;
});
```

output:
```js
// 15
```


[forEach-helper]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach
