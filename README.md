# MongoDB $inc Operator Issue

This repository demonstrates an issue encountered when using the `$inc` operator in MongoDB.  Incorrectly using a negative value with `$inc` can lead to negative counter values.

The `bug.js` file shows the problematic code.  The `bugSolution.js` file provides a corrected approach.

## Solution
The solution involves adding a check to ensure the counter doesn't decrement below zero. 