# MongoDB $inc operator error
This repository demonstrates a common error when using the $inc operator in MongoDB. The $inc operator is used to increment a numerical field by a specified value. However, it is important to ensure that the value being incremented is a number.  Using a string will result in an error.

## Bug
The bug is in the `updateOne` method. The `$inc` operator is used with a string value ('1') instead of a numerical value (1). This will cause the update to fail. 

## Solution
The solution is to provide a numerical value instead of a string to the $inc operator.