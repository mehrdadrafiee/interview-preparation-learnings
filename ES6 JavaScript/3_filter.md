# filter()

[`filter`][filter-helper] helper produces a subset (**creates a new array**) of all the records that pass the test implemented by the provided function.

```js
let products = [
  { name: 'cucumber', type: 'vegetable', quantity: 0, price: 3 },
  { name: 'banana', type: 'fruit', quantity: 4, price: 4 },
  { name: 'celery', type: 'vegetable', quantity: 12, price: 2 },
  { name: 'orange', type: 'fruit', quantity: 5, price: 6 }
];

products.filter((product) => {
  return product.type === 'fruit';
});
```

```js
// 'products' array                                                    result array

// fruit ---------> Iterator Function ----returns----->true ---------> fruit
// vegetable ---------> Iterator Function ----returns----->false
// fruit ---------> Iterator Function ----returns----->true ---------> fruit
```

---

### Example(s)

```js
let post = { id: 4, title: 'New Post' };
let comments = [
  { postId: 4, content: 'awesome post' },
  { postId: 3, content: 'it was ok' },
  { postId: 4, content: 'neat' }
];

function commentsForPost(post, comments) {
  return comments.filter(function(comment) {
    return comment.postId === post.id;
  });
}

// [{ "postId":4, "content":"awesome post" }, { "postId":4, "content":"neat" }]
```

```js
let numbers = [15, 25, 35, 45, 55, 65, 75, 85, 95];

let filteredNumbers = numbers.filter((number) => {
  return number > 50;
});

console.log(filteredNumbers);

// [55, 65, 75, 85, 95]
```

[filter-helper]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter
