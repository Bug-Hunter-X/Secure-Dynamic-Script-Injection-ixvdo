# Uncommon HTML Bug: XSS Vulnerability from innerHTML

This repository demonstrates a subtle yet dangerous HTML bug related to using `innerHTML` to dynamically add script tags.  Improper use can lead to Cross-Site Scripting (XSS) vulnerabilities.

The `bug.html` file shows the problematic code.  The `solution.html` file presents a safer alternative using DOM manipulation.

## Bug Description

Directly inserting script tags using `innerHTML` can create a security risk.  Malicious code injected into the innerHTML could execute in the user's browser.

## Solution

The solution avoids this by correctly creating the script element and appending it to the DOM, preventing XSS vulnerabilities.