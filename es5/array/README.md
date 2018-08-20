# ES5 Arrays

## Useful Methods

**Fill an array of set length**

```js
const populateArray = (length, callback) => {
  Array(length).fill().map(callback);
}

console.log(populateArray(5, (_, i) => i));
// => [0, 1, 2, 3, 4]
```
