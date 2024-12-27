# Inconsistent Rendering with CSS calc() Function

This repository demonstrates a subtle bug related to the unexpected behavior of the `calc()` function in CSS, particularly when used with multiple units and nested elements. The bug manifests as inconsistent rendering across different browsers and can be challenging to debug.

The `bug.css` file contains the problematic CSS code, while `bugSolution.css` provides a corrected version with a workaround to ensure consistent rendering.

## Bug Description
The `calc()` function in CSS allows for dynamic calculation of values. However, unexpected behavior can occur when combining percentage and pixel values in specific scenarios.  The core issue is that the order of operations and unit handling within `calc()` might vary slightly across different browser implementations. This is more prevalent in nested contexts.

## Solution
The solution avoids relying solely on `calc()` for complex calculations where multiple units are used. The corrected code uses a more robust approach that consistently produces the intended layout across various browsers and contexts. 