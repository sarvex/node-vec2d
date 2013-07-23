# vec2d

Node.js 2d vector library

## Usage

```js
var v = require('vec2d');

var v1 = v(1, 2);
console.log(v1); // prints "(1, 2)"

var v2 = v1.offset(1, 0);
console.log(v2); // prints "(2, 2)"

var v3 = v({x: -1, y: 2.2});
console.log(v3); // prints "(-1, 2.2)"
```

Or a faster, less convenient version:

```js
var Vec2d = require('vec2d').Vec2d;

var v1 = new Vec2d(1, 2);
// etc...
```

More available functions are listed below in Test Coverage.

## Test Coverage

```
  v()
    ✓ no args 
    ✓ x, y 
    ✓ array 
    ✓ object 
    ✓ string coords 
    ✓ deserialize 
    ✓ invalid deserialize 

  Vec2d
    ✓ offset 
    ✓ add 
    ✓ sub 
    ✓ plus 
    ✓ minus 
    ✓ neg 
    ✓ mult 
    ✓ times 
    ✓ div 
    ✓ divBy 
    - scale
    - scaled
    - clone
    - apply
    - applied
    - equals
    - toString
    - length
    - lengthSqrd
    - angle
    - normalize
    - normalized
    - boundMin
    - boundMax
    - floor
    - floored
    - ceil
    - ceiled
    - project
    - dot
    ✓ rotate 
    - rotated
    - distance
    - distanceSqrd


  41 tests complete (10 ms)
  23 tests pending
```

More functions welcome in the form of pull requests.
