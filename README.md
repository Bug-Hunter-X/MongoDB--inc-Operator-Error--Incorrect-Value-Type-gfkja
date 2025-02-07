# MongoDB $inc Operator Error: Incorrect Value Type

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The `$inc` operator is designed to increment a numeric field by a specified value. However, providing a string value instead of a number will lead to unexpected results or errors.

## Bug Description
The provided JavaScript code snippet attempts to increment the `field` of a document where `_id` is 1 by the value '1' (a string), which is incorrect. The correct usage requires a numerical value.

## Solution
The solution involves ensuring that the value passed to the `$inc` operator is a number. The corrected code snippet is included in `bugSolution.js`.