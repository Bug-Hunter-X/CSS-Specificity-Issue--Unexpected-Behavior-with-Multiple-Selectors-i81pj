# CSS Specificity Bug

This repository demonstrates a subtle bug related to CSS selector specificity and the order in which the browser applies styles.  The bug occurs when multiple selectors target the same element, and the specificity rules aren't entirely clear.  The solution provides a fix to ensure the intended styling is applied.

## Bug Description
The issue stems from a potentially unexpected interaction between the `#myElement` selector (ID selector, high specificity) and `.myClass` selector (class selector, lower specificity), when an element has both an ID and a class.

## Setup
1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Observe that the element's background color is blue, even though the ID selector's rule should take precedence.

## Solution
The solution involves careful management of CSS selector specificity and order to guarantee the desired style is applied.  Review `bugSolution.css` for the correct implementation.