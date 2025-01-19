# React Unhandled Empty Array Response from API

This repository demonstrates a common error in React applications when handling API responses: failure to gracefully handle empty array responses.

The `bug.js` file contains the buggy code which attempts to render a list from API data without checking for an empty array.  This results in an error. The `bugSolution.js` file provides the corrected code which properly handles the case of an empty array. 

## How to reproduce the bug

1. Clone this repository.
2. Run `npm install`
3. Run `npm start` (Assumes you have a mock API serving an empty array for the specified endpoint)
4. Observe the error in the console.

## How to fix the bug

Refer to `bugSolution.js` for the corrected code.  The solution involves checking if the `data` array is empty before attempting to map over it.