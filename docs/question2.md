 # Explain the output of the above-given code and explain why?

```for (var i = 0; i < 5; i++) {

  setTimeout(() => console.log(i), 100)

}
```
## ANS:

The output of the code will be 5 5 times.

The reason for this is because the setTimeout() function is asynchronous. This means that it does not execute immediately. Instead, it is scheduled to execute after 100 milliseconds. By the time the setTimeout() function executes, the value of i has already been incremented to 5.

Since the setTimeout() function has access to the value of i from the outer function, it will log the value of i as 5, even though the value of i in the inner function is still 0.

the setTimeout() function will log the value of i that was in scope when it was called, even if that value has changed by the time the function actually executes.
