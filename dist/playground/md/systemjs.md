```js
// geometry/Shape.js
System.register("geometry/Shape", [], function (exports, context) {
    var Shape;
    return {
        setters: [],
        execute: function() {
            Shape = (function(){
                // ...
                return Shape;
            }());
            exports("Shape", Shape)
        }
    };
});

// index.js
System.register("index", ["geometry/Shape"], function (exports, context) {
    var Shape;
    return {
        setters: [
            function (Shape_1) {
                Shape = Shape_1;
            }
        ],
        execute: function() {
            var a = new Shape("shape1", 100, 200);
        }
    }
});
```