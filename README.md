# Inconsistent :focus-visible Pseudo-class Behavior

This repository demonstrates a common issue with the CSS `:focus-visible` pseudo-class.  Some browsers exhibit inconsistent behavior, leading to accessibility problems and unexpected visual feedback for focused elements.

## Problem

The `:focus-visible` pseudo-class is intended to provide a visual indicator only when an element receives focus and is *not* programmatically focused (e.g., via JavaScript). However, implementation inconsistencies across browsers mean that the styling may not consistently apply. 

The `bug.css` file contains code that exemplifies the problem.  You will likely see different results depending on your browser.

## Solution (bugSolution.css)

This issue doesn't have a simple fix in pure CSS. A robust solution often involves JavaScript to handle focus events more precisely. This is demonstrated in bugSolution.css, which shows how to manually trigger visual changes, ensuring that accessibility is improved and there's visual consistency across different browsers.