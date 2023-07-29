# What will the code below output to the console and why?

```var arr1 = "john".split(''); 

var arr2 = arr1.reverse();

var arr3 = "jones".split('');

arr2.push(arr3);

console.log("array 1: length=" + arr1.length + " last=" + arr1.slice(-1));

console.log("array 2: length=" + arr2.length + " last=" + arr2.slice(-1));
```
## ANS:
The code will output the following to the console:
```
array 1: length=5 last=s
array 2: length=5 last=j,o,n,e,s
```

Explanation:

- `arr1` and `arr2` refer to the same reversed array `['n', 'h', 'o', 'j']`.
- `arr2.push(arr3)` adds `arr3` as a single element at the end of `arr2`.
- Printing `arr1.slice(-1)` gives the last element of `arr1`, which is "s".
- Printing `arr2.slice(-1)` gives the last element of `arr2`, which is the array `['j', 'o', 'n', 'e', 's']`.
