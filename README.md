# demo-extract-css
Let's say we have 2 JS modules,  import('B.js') in A.js, import 'B.css' in B.js, and what I want to get is 2 files: A.js, B.js(containing content of B.css), rather than outputing 3 files: A.js, B.js, B.css.

Since all CSS files have been extracted to individual CSS files, when the async modules load the extracted CSS files, the browser will have to make extra request for the CSS files.
