# Uncommon HTML Bug: Accessing Non-Existent Element

This repository demonstrates a subtle bug in HTML/JavaScript related to accessing DOM elements that do not exist. The bug is subtle because it doesn't throw a noticeable error, but silently fails to update the webpage as expected.  Understanding how to properly check for the existence of DOM elements is crucial for robust web development.

## Bug Description

The `bug.html` file contains a script that attempts to modify the `innerHTML` of an element with the ID `myDiv2`. However, the HTML only contains an element with the ID `myDiv`. This leads to the script failing silently, with no visible error message to guide the developer.

## Solution

The `bugSolution.html` demonstrates a corrected version of the script. It uses a conditional check to verify the existence of the element before attempting to modify it.  This avoids potential runtime errors and ensures the script executes correctly, even if the targeted element is missing.

## How to reproduce

1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe that the text within the div does not change.
4. Open `bugSolution.html`. The text should correctly update.  Check your browser's console for error messages in `bug.html`
