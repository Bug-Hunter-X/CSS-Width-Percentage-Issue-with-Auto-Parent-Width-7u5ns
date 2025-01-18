# CSS Width Percentage Issue

This repository demonstrates an uncommon CSS bug related to using percentage widths when the parent container's width is not explicitly set.  The bug manifests as unexpected behavior in some browsers where elements with percentage widths do not correctly take up the expected proportion of the parent's width.

The `bug.css` file contains the problematic code. The `bugSolution.css` file provides a solution.

## Bug Description
When a child element's width is set using a percentage (e.g., `width: 50%;`) and its parent container does not have an explicitly defined width (e.g., `width: 100%;`, `width: 500px;`, etc.), the child element's width may not behave as expected across different browsers. The percentage will be relative to the parent's width, but if the parent's width is `auto`, interpretations differ.