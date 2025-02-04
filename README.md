# Uncommon HTML Bug: Handling Non-Existent Element Access

This repository demonstrates a common but often overlooked error in HTML: attempting to access a non-existent element by its ID without proper error handling.  The `bug.html` file contains the buggy code, while `bugSolution.html` provides the corrected version.

## Bug Description

The bug arises from directly accessing an element's properties (e.g., `innerHTML`) via `getElementById` without first checking if the element exists.  If the element with the specified ID is not found, this will result in an error, crashing the script.

## Solution

The solution involves checking if `getElementById` returns `null` before attempting any operations on the element.  This prevents errors and ensures the script handles the case where the element is absent gracefully.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in a web browser.  You'll observe an error in the browser's console.
3. Open `bugSolution.html`.  This version correctly handles the potential absence of the element.