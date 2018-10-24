# Coverage Weirdness in Node.js

For some of the internal modules in Node.js, it seems that the coverage reported
by the inspector does not include the outer most block:

<img src="./images/top-level-not-covered.png" />

This should nont be possible, given that it does contain coverage for deeper
blocks within the AST.
