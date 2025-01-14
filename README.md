# CSS Specificity Bug

This repository demonstrates a common CSS issue related to selector specificity. The goal is to style paragraphs inside a container differently than paragraphs outside the container. However, due to CSS specificity rules, the styling of the paragraphs within the container unintentionally overwrites the general styling for paragraphs.

## Problem

The 'container p' selector has higher specificity than the 'p' selector.  This means that any styles defined for 'container p' will override styles defined for 'p', even if the 'p' selector is declared later.

## Solution

The solution involves using more specific selectors for the general paragraph styles or utilizing the `!important` flag (although this is generally discouraged).