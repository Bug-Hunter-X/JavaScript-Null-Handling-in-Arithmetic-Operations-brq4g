# JavaScript Null Handling Bug

This repository demonstrates a common, yet subtle, bug in JavaScript related to handling null values in arithmetic operations.  The `foo` function attempts to add two numbers, but it doesn't robustly handle null inputs.

## Bug Description
The function `foo` returns null if either `a` or `b` is null. While this seems correct for strictly numerical addition, it doesn't handle cases where null might represent a missing or zero value.  In some scenarios, this behavior might lead to unexpected results or errors in a larger application.

## How to Reproduce
1. Clone this repository.
2. Open `bug.js` and run the code using a JavaScript interpreter (Node.js, browser console, etc.).
3. Observe the output; note the behavior when one or both inputs are null.

## Solution
The solution involves adding more robust null handling, allowing more flexibility in how null values are interpreted. See `bugSolution.js` for the corrected version.