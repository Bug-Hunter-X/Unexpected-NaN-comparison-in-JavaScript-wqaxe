# Unexpected NaN comparison in JavaScript

This repository demonstrates a common, yet subtle, error in JavaScript related to comparing NaN (Not a Number) values.

The strict equality operator (===) in JavaScript is known to return false when comparing NaN with itself.  This counter-intuitive behavior can lead to unexpected results and bugs in your code. This repo contains two files: bug.js which illustrates the error and bugSolution.js shows a better way to handle the scenario.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js` and run the code using Node.js or a similar JavaScript runtime.
3. Observe that even though both variables are NaN, the strict comparison returns `false`.

## Solution

Refer to `bugSolution.js` for a solution using the isNaN() method.  This provides a more robust and reliable way to detect NaN values.