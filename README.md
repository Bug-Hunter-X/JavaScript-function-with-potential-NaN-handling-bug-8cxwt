# JavaScript Function with NaN Handling Bug

This repository demonstrates a common yet subtle bug in JavaScript functions involving the handling of NaN (Not a Number) values.

## Bug Description
The `foo` function adds two numbers.  It correctly handles `null` inputs but fails to explicitly check for `NaN`. If either input is `NaN`, the result of the addition will be `NaN`, potentially causing unexpected errors in applications that use this function.

## Bug Solution
The improved `foo` function explicitly checks for `NaN` values using `isNaN()` before performing the addition.  If either input is `NaN`, the function returns 0, providing a more robust solution.

## How to reproduce
1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` in your preferred text editor.
3. Execute the JavaScript files in a Node.js environment or a browser's console to observe the original bug's behavior and the corrected version's output.