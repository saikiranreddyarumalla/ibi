#  What will the following code's output be in sequence and explain why?
```function printNumber(num) {
  console.log(num);
}
console.log(1);
setTimeout(printNumber, 0, 2);
setTimeout(printNumber, 100, 3);
console.log(4);
```
# ANS:
The output sequence will be: `1`, `4`, `2`, `3`.
## Explanation:
- `1` is logged immediately when `console.log(1);` is executed.
- `4` is logged immediately when `console.log(4);` is executed.
- `2` is logged next after the synchronous part of the code is finished, but before `3`, as it has a 0ms delay in `setTimeout`.
- `3` is logged last after a 100ms delay in `setTimeout`.
