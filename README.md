# Loose Equality in JavaScript
This repository demonstrates a common error in JavaScript: the unexpected behavior of loose equality (`==`) when dealing with `null` and `undefined` values.

The file `bug.js` contains code that exhibits the issue.  `bugSolution.js` provides the corrected code using strict equality (`===`).

## Problem
Loose equality performs type coercion before comparison, which can lead to unexpected results.  In particular, `null == undefined` evaluates to `true`, while `null === undefined` evaluates to `false`.

This difference can cause subtle bugs that are difficult to detect.

## Solution
Always use strict equality (`===`) when comparing values in JavaScript to avoid type coercion and ensure accurate comparisons.

This ensures that both the value and the type are compared, preventing the unexpected results associated with loose equality.