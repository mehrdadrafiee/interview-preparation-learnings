### forEach

`forEach` is and array helper method. We have access to `forEach` method on any given array. We pass in an anonymous function to the `forEach` helper which gets called one time for every element in the array and whatever is inside the function would be executed.

```js
let colors = [ 'red', 'green', 'blue' ];

colors.forEach(function(color) {
  console.log(color);
});
```

output:
```js
// red
// green
// blue
```
