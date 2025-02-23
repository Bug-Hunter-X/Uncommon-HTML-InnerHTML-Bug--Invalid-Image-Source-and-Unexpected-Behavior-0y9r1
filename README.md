# Uncommon HTML Bug: Handling InnerHTML Incorrectly

This repository demonstrates a subtle bug related to modifying the `innerHTML` property of an HTML element.  The primary issue lies in concatenating strings directly into `innerHTML` without proper sanitization and error handling. This can lead to unexpected behavior and security vulnerabilities if the content being added is not fully trusted.

The solution shows the safe way to modify the `innerHTML` property and use proper DOM manipulation techniques.

## Bug

The `bug.html` file contains the buggy code.  The issue is in the script that directly concatenates a paragraph element and an image element into the `innerHTML` of a div. Because the image source ('nonexistent.jpg') is invalid, it causes an error. This is an example of how unexpected content in `innerHTML` can cause problems.

## Solution

The `bugSolution.html` file demonstrates a safer approach: creating the elements correctly and setting their attributes, thereby avoiding unexpected behavior and security risks.