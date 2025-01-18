# Uncommon HTML Bug: Incorrect Element Selection

This repository demonstrates a common yet easily missed error in JavaScript when selecting HTML elements by ID using `document.getElementById()`.  The issue lies in incorrectly including the '#' symbol within the ID selector.

## Bug Description
The bug is in the javascript. The `document.getElementById()` method should receive the id value and not the CSS selector of the element. The '#' symbol should not be included in the argument passed to `document.getElementById()`. 

## Solution
The solution involves correctly using `document.getElementById()` without the '#' symbol in the selector string.

## How to reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe that the div element is not hidden because the incorrect selector is used in `document.getElementById()`.
4. Open `bugSolution.html` to see the corrected code.
