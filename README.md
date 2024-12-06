# CSS `calc()` Issue in Flexbox

This repository demonstrates a problem with the CSS `calc()` function when used within a flexbox container, specifically when performing subtraction.

The `bug.css` file contains the problematic code. The `bugSolution.css` file offers a corrected approach.

## Problem Description

When using `calc()` to subtract a value (e.g., `calc(100% - 10px)`) to determine the width of an element within a flexbox container that does not have its width explicitly set, the calculation may not produce the expected result.

## Solution

To resolve the issue, ensure that the parent flex container has a defined width.  This provides a stable base for the `calc()` function to operate correctly.