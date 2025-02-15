# JavaScript Loose Comparison Bug

This repository demonstrates a common error in JavaScript related to loose comparison using the `==` operator. The `foo` function checks for equality between two values, but it can produce unexpected results due to type coercion performed by the loose comparison. 

## Bug Description
The `foo` function uses loose comparison (`==`) to check if two inputs are equal. Loose comparison can lead to unexpected results when comparing values of different types. For example `1 == '1'` evaluates to `true`, even though they are of different types.  This can introduce subtle bugs that are difficult to detect.

## Solution
The recommended practice is to use strict equality (`===`) whenever possible to avoid type coercion. Strict equality checks for both value and type, resulting in more predictable and reliable behavior.  The solution provides a corrected `foo` function using strict equality.

## How to Run
1. Clone the repository.
2. Open `bug.js` and `bugSolution.js` in your preferred JavaScript environment.
3. Execute the functions and observe the difference in output.