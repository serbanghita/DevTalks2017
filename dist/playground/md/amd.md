```js
// geometry/Shape.js
define("geometry/Shape", ["require", "exports"], function (require, exports) {
    var Shape = (function () {
        // ...
        return Shape;
    }());
    exports.Shape = Shape;
});

// index.js
define("index", ["require", "exports", "geometry/Shape"], function (require, exports, Shape) {
    var a = new Shape("shape1", 100, 200);
});
```