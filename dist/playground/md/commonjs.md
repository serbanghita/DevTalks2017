```js
// geometry/Shape.js
var Shape = (function () {
    // ...
    return Shape;
}());
exports.Shape = Shape;

// index.js
var Shape = require("./geometry/Shape");
var a = new Shape("shape1", 100, 200);
```