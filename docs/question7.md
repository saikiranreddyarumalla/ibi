# Use Array.reduce() method to reverse the following given array

```const arr = [1, 2, 3, 4, 5] ```
## ANS:
To reverse the given array using the `Array.reduce()` method, you can do the following:

```javascript
const arr = [1, 2, 3, 4, 5];

const reversedArr = arr.reduce((acc, curr) => {
  acc.unshift(curr);
  return acc;
}, []);

console.log(reversedArr); // Output: [5, 4, 3, 2, 1]
```

In the above code, we start with an empty array (`[]`) as the initial value for the accumulator. Then, we use the `unshift()` method to add each element from the original array to the beginning of the accumulator. The result is a reversed array stored in `reversedArr`.
