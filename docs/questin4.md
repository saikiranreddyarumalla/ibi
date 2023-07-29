# What is promise chaining? Explain with an example.
## ANS:
promise chaining is a way to execute multiple asynchronous tasks one after the other using `.then()`. Each task depends on the successful completion of the previous one. This ensures a sequential flow and makes the code more organized.
### Example:
#### javascript
fetchData()
  .then(processData)
  .then(saveData)
  .then((result) => {
    console.log("Final result:", result);
  })
  .catch((error) => {
    console.error("Error occurred:", error);
  });
```

In this example, `fetchData`, `processData`, and `saveData` are asynchronous functions returning Promises. They are executed in sequence, and the final result is logged to the console. If any promise in the chain rejects, the error is caught in the `.catch()` handler.
