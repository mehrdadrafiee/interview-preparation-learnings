# map

`map`[map-helper] helper is the most widely used array helper. The `map()` method **creates a new array** with the results of calling a provided function on every element in the calling array.

```js
let numbers = [ 1, 2, 3 ];
let doubledNumbers = [];

let doubled = numbers.map((number) => {
  return number * 2;
});

// [2, 4, 6]
```

'numbers' array                                    result array

1 ---------> Iterator Function ----_returns_-----> 2
2 ---------> Iterator Function ----_returns_-----> 4
3 ---------> Iterator Function ----_returns_-----> 6

### Example(s)

```js
let cars = [
  { model: 'Tesla', price: 'expensive' },
  { model: 'Toyota', price: 'cheap' }
];

let prices = cars.map((car) => {
  return car.price;
});

// ['expensive', 'cheap']
```

---

```js
let trips = [
  { distance: 34, time: 10 },
  { distance: 90, time: 50 },
  { distance: 59, time: 25 }
];

let speeds = trips.map(({ distance, time }) => {
  return distance / time;
});

// [3.4, 1.8, 2.36]
```


[map-helper]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map
