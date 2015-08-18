# FTrig

FTrig is a utility for fast approximate trigonometric calculating on javascript,
based on [this article](http://lab.polygonal.de/?p=205).
FTrig can be used with [Node.js](http://nodejs.org), 
[RequireJS](http://requirejs.org/) or directly in the browser.

A FTrig instance is create as:
```javascript
var trig = new FTrig(FTrig.LOW); // faster, less accurate
// or
var trig = new FTrig(FTrig.HIGH); // more, more accurate

trig.sin(Math.PI/4);
trig.cos(Math.PI/4);
```

A FTrig instance provides 2 functions: `sin` and `cos`, as alias of the 4 main functions:
`sinLow`, `cosLow` for `FTrig.Low` and `sinHigh`, `cosHigh` for `FTrig.High`.

## Download

The source is available for download by cloning.
Alternatively, you can install via:

- [npm](https://www.npmjs.com/): `To be updated`
- [bower](http://bower.io/): `To be updated`

## In the Browser

Usage:

```html
<script type="text/javascript" src="FTrig.js"></script>
<script type="text/javascript">

    var trig = new FTrig(FTrig.LOW);
    trig.sin(Math.PI/4);

</script>
```