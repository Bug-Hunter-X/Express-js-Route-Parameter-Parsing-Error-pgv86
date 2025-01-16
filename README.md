# Express.js Route Parameter Parsing Error

This repository demonstrates a common error in Express.js applications related to parsing route parameters and provides a solution.

## Bug Description
The bug lies in the lack of robust error handling when parsing a numerical route parameter.  The code attempts to convert the parameter to an integer using `parseInt`, but it doesn't handle cases where the parameter is not a valid integer, leading to potential crashes or unexpected results.

## Solution
The solution involves adding comprehensive error handling. This includes checking if `parseInt` returns `NaN` and providing appropriate responses for invalid parameters.