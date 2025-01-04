# CSS nth-child issue with nested lists

This repository demonstrates a common issue with the `:nth-child` selector in CSS when dealing with nested lists. The `bug.css` file contains the problematic code, while `bugSolution.css` offers a solution.

## Problem

The `:nth-child(odd)` and `:nth-child(even)` selectors, while useful for alternating styles, only apply to the *direct* children of an element. When nested lists are involved, the styling is not consistently applied to all list items.

## Solution

The solution utilizes a more robust approach that recursively styles the list items, ensuring consistent alternating background colors regardless of list nesting levels.  This is achieved using a recursive selector approach or counter-based methods (as demonstrated in `bugSolution.css`).