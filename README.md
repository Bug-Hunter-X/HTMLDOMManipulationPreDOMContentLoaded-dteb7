# Uncommon HTML Error: DOM Manipulation Before Load

This repository demonstrates a subtle but common error in HTML/JavaScript: attempting to manipulate the DOM (Document Object Model) before the page's DOM is fully loaded. This frequently leads to unexpected behavior, such as elements not being found or styles not applying.

The `bug.html` file showcases the faulty code, while `bugSolution.html` presents a corrected version that utilizes the `DOMContentLoaded` event listener to ensure DOM manipulation occurs only after the DOM is ready.

## How to Reproduce the Bug

1. Open `bug.html` in a web browser.
2. Observe that the text within the `div` element is not hidden as intended.  This is because the JavaScript attempts to access the element before it exists in the DOM.

## Solution

The solution in `bugSolution.html` uses the `DOMContentLoaded` event listener. This ensures that the JavaScript code executes only after the entire page's HTML is parsed and the DOM is ready for manipulation.