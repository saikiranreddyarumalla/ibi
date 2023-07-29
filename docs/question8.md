# In what order will the numbers 1-4 be logged to the console when the code below is executed? Why?

```(function() {

    console.log(1); 

    setTimeout(function(){console.log(2)}, 1000); 

    setTimeout(function(){console.log(3)}, 0); 

    console.log(4);

})();
```

## ANS:
The numbers 1, 4, 3, and 2 will be logged to the console in the order: 1, 4, 3, 2.

```console.log(1)``` logs 1 immediately as it's synchronous code.
```console.log(4)``` logs 4 immediately after 1.
```setTimeout(function(){console.log(3)}, 0);``` logs 3 after a brief delay, even though the delay is set to 0, because it's scheduled in the callback queue after the synchronous code.
```setTimeout(function(){console.log(2)}, 1000);``` logs 2 after a 1-second delay since it's scheduled in the callback queue after the 0-ms delay setTime
