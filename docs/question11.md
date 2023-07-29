# Check the below given code, if there are any issues, fix them and explain the output

```const numbers = [1, 2, 3, 4, 5];
const result = numbers.reduce((acc, num) => {
  if (num % 2 === 0) {
    acc.evens.push(num);
  } else {
    acc.odds.push(num);
  }
  return acc;
});
console.log(result);
```
## ANS:
- The given code has a missing initial value for the accumulator in the reduce() function. 
- We'll fix it by providing an object with evens and odds properties as the initial value. 
- The code separates even and odd numbers from the numbers array and returns an object with the results.

```const numbers = [1, 2, 3, 4, 5];
const result = numbers.reduce((acc, num) => {
  if (num % 2 === 0) {
    acc.evens.push(num);
  } else {
    acc.odds.push(num);
  }
  return acc;
}, { evens: [], odds: [] });
console.log(result);
```
The output will be:
```{ evens: [2, 4], odds: [1, 3, 5] }```
