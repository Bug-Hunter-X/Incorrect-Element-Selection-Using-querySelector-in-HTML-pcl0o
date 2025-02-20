# Uncommon HTML Bug: Incorrect Element Selection

This repository demonstrates a common yet subtle error in JavaScript when interacting with the DOM (Document Object Model) in an HTML file.
The bug involves the use of `document.querySelector` to select an element and then modifying its style.  In this case, the selected element is correctly referenced however the element's visibility is incorrectly modified and the element is not found.

## Bug Description
The provided HTML code attempts to hide a div element using JavaScript.  However, there is a minor error in how the element is selected, leading to unexpected behavior.

## Solution
The solution involves correctly using `document.getElementById("myDiv")` to select the element by its ID, this is considered best practice.  This ensures that the correct element is targeted for modification.
