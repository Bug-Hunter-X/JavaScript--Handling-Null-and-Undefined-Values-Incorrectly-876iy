# JavaScript: Handling Null and Undefined Values Incorrectly

This repository demonstrates a common JavaScript error related to handling null and undefined values. The `bug.js` file contains code that attempts to handle null values, but fails to handle undefined, resulting in a `TypeError`.  The `bugSolution.js` file provides a corrected version.

## Problem
The original code uses a loose equality check (`==`) to determine if a value is null. While this handles null correctly, it does not handle the case where the input is `undefined`. Attempting to access the `length` property of `undefined` throws a `TypeError`.

## Solution
The solution uses strict equality (`===`) to check for both null and undefined values, providing a more robust and accurate handling of potentially missing data.  This ensures the code functions correctly regardless of whether the input is null or undefined.