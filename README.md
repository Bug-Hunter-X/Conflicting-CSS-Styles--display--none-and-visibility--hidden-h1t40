# Conflicting CSS Styles: display: none and visibility: hidden

This repository demonstrates an uncommon HTML bug involving conflicting CSS styles that unexpectedly hide an HTML element.

The bug occurs when both `display: none` and `visibility: hidden` styles are applied to the same element simultaneously.  While both styles hide the element, their effects are different and they might conflict, leading to unexpected and harder-to-debug behavior.

## Bug Description:
The HTML file contains a simple div element. The JavaScript code applies both `display: none` and `visibility: hidden` styles, resulting in the div element being completely hidden. While the intention is to hide the element, using both styles together is redundant and can create unexpected issues in more complex scenarios.

## How to Reproduce:
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe that the div element with the id "myDiv" is not visible despite containing text.

## Solution:
The solution involves removing the redundant style. Using either `display: none` or `visibility: hidden` is sufficient to hide the element.