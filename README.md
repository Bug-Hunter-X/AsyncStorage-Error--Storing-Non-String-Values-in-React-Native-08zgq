# AsyncStorage Error: Storing Non-String Values in React Native

This repository demonstrates a common error in React Native when using AsyncStorage to store data types other than strings. AsyncStorage only supports strings, so attempting to store objects, numbers, or other data structures will lead to unexpected behavior or silent failures.

The error itself is not always explicit, making it difficult to debug.

## Bug Reproduction

The `bug.js` file shows the erroneous code that attempts to store a JavaScript object in AsyncStorage. Run the application and observe the result.  The application might crash or exhibit unexpected behavior.

## Solution

The `bugSolution.js` file demonstrates the correct approach, converting objects into strings using `JSON.stringify()` before storage and parsing them back using `JSON.parse()` upon retrieval.