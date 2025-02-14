# Uncommon HTML Bug: innerText vs. textContent

This repository demonstrates a subtle bug related to manipulating the text content of HTML elements using JavaScript.  Specifically, it highlights the difference between `innerText` and `textContent` and the potential pitfalls of using the wrong property.

The `bug.html` file contains the incorrect code, while `bugSolution.html` shows the corrected version.

**The Problem:**

Incorrectly using `textContent` when dealing with rich text content can lead to unexpected behavior. `textContent` includes all text nodes, including those within HTML tags, while `innerText` only includes the visible text content. If the HTML structure has multiple levels of tags, then the textContent will return all the text content, whereas the innerText returns the content displayed in the browser.