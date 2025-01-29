# Ada Array Copy Issue

This example demonstrates a potential confusion when copying arrays in Ada.  Modifying a copy of an array appears to modify the original, which is not the expected behavior.

The `bug.ada` file contains code demonstrating this issue. The solution in `bugSolution.ada` shows how to correctly copy the array.

## Problem
The initial code creates an array `A` and a copy `B`.  Altering `B` unexpectedly affects `A`.

## Solution
The solution uses an explicit loop to create a true copy of the array, ensuring that changes to the copied array do not affect the original.