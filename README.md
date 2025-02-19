# CSS Pseudo-element Content Rendering Issue
This repository demonstrates an uncommon bug related to CSS pseudo-elements (`:before`, `:after`) and the handling of special characters within their `content` property.

## Bug Description
When using pseudo-elements with content that includes special characters (single quotes, double quotes, etc.), unexpected rendering or errors may occur in certain browsers.  This is not a consistently reproducible issue across all browsers and versions, making it difficult to debug.

## Solution
The solution involves escaping the special characters within the content string, or using alternative methods like using `attr()` to fetch content from an attribute, which avoids these kind of issues.