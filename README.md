# Uncommon HTML Bug: Multiple innerHTML Appends

This repository demonstrates an uncommon bug in HTML related to the use of `innerHTML` to append multiple elements to a container.  Improper use of `innerHTML` in this manner can lead to unexpected behavior and security risks. This example showcases the bug and provides a solution.

## Bug Description:

The bug occurs when multiple calls to `innerHTML +=` are used to append multiple HTML elements to a single container element. Subsequent calls overwrite preceding elements. This can lead to losing some of the intended elements or unexpected formatting.

## Solution:

Instead of using `innerHTML +=` multiple times, use a single call to `innerHTML` to append all the necessary HTML.  Alternatively, use DOM manipulation methods such as `appendChild` or `insertBefore` for better control over the structure and reduces the risk of vulnerabilities.