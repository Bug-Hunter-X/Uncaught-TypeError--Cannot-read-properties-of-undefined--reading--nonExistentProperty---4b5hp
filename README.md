# Uncommon HTML/JS Bug: Accessing Non-Existent Element Properties

This repository demonstrates a common yet easily overlooked error in JavaScript when interacting with HTML elements: attempting to access a property that doesn't exist on the element object.  This typically results in a `TypeError: Cannot read properties of undefined (reading 'propertyName')` error.

## The Bug
The `bug.html` file contains a simple HTML structure with a `<div>` element. The JavaScript code attempts to access a property (`nonExistentProperty`) that is not defined for the `myDiv` element. This causes a runtime error.

## The Solution
The `bugSolution.html` file shows the corrected version.  Before accessing properties, it's essential to verify that the element exists and that the property you intend to access is defined.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser. You will observe the JavaScript error in the console.
3. Open `bugSolution.html`; this version handles the potential error, preventing the crash and handling missing properties gracefully.