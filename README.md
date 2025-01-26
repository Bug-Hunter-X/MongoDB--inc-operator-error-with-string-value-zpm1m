# MongoDB $inc operator error with string value
This example demonstrates an uncommon error when using the `$inc` operator in MongoDB update operations. The error occurs when a string value is provided to the `$inc` operator instead of a numeric value. 

## Bug Description
The provided code attempts to increment the 'age' field of a document by '1', but '1' is passed as a string which causes an error.

## Solution
The bug is solved by ensuring that the value incremented by $inc is a number (integer or float).