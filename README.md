# MongoDB $inc Operator Bug

This repository demonstrates an uncommon bug related to the `$inc` operator in MongoDB update queries. The bug arises from using a string instead of a number as the increment value.

## Bug Description
The `$inc` operator is used to increment a numerical field in a MongoDB document. When a string is used instead of a number, the update operation will fail to increment the field correctly.

## Bug Reproduction
1. Clone this repository.
2. Run the `bug.js` script.
3. Observe that the `count` field is not correctly incremented in the MongoDB collection.

## Bug Solution
The `bugSolution.js` script shows the correct implementation of the update query, using a numerical value with the `$inc` operator.