`__proto__` is the actual object that is used in the lookup chain to resolve methods, etc. 
`prototype` is the object that is used to build `__proto__` when you create an object with `new`:

```js
( new Shape ).__proto__ === Shape.prototype
( new Shape ).prototype === undefined
```