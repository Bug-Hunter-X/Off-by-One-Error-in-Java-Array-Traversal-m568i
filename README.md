# Off-by-One Error in Java Array Traversal

This repository demonstrates a common off-by-one error in Java when iterating over arrays. The buggy code attempts to access an array element beyond its valid index, leading to an `ArrayIndexOutOfBoundsException`. The solution shows how to correct the loop condition to prevent this error.

## Bug Description

The `BuggyArray.java` file contains a `for` loop that iterates one element beyond the array's bounds.  This results in an exception when the code attempts to access `arr[5]` (index 5) of an array with only 5 elements (indices 0-4).

## Solution

The `FixedArray.java` file shows the corrected code. The loop condition is changed to `i < arr.length`, ensuring the loop stops before attempting to access an invalid index.

## How to Run

1. Clone this repository.
2. Compile and run `BuggyArray.java` to observe the `ArrayIndexOutOfBoundsException`. 
3. Compile and run `FixedArray.java` to see the corrected output.