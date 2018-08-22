# tiles-in-bbox
Get all tiles of a web map in x,y,z coordinates for a specified bounding box and zoom.


## Installation
`npm install tiles-in-bbox`

## Usage

``` javascript
var t = require('tiles-in-bbox')

//Follows the GeoJson/OpenStreetMaps convention of a clockwise box starting at the bottom.
var bbox = {
    bottom : 42.356,
    left : -71.1279,
    top : 42.3876,
    right : -71.1002,
}

var zoom = 15
var tiles = t.tilesInBbox(bbox, zoom)
console.log(tiles)
```

## Results
```javascript
[ { x: 9909, y: 12116, z: 15 },
  { x: 9909, y: 12117, z: 15 },
  { x: 9909, y: 12118, z: 15 },
  { x: 9909, y: 12119, z: 15 },
  { x: 9909, y: 12120, z: 15 },
  { x: 9910, y: 12116, z: 15 },
  { x: 9910, y: 12117, z: 15 },
  { x: 9910, y: 12118, z: 15 },
  { x: 9910, y: 12119, z: 15 },
  { x: 9910, y: 12120, z: 15 },
  { x: 9911, y: 12116, z: 15 },
  { x: 9911, y: 12117, z: 15 },
  { x: 9911, y: 12118, z: 15 },
  { x: 9911, y: 12119, z: 15 },
  { x: 9911, y: 12120, z: 15 },
  { x: 9912, y: 12116, z: 15 },
  { x: 9912, y: 12117, z: 15 },
  { x: 9912, y: 12118, z: 15 },
  { x: 9912, y: 12119, z: 15 },
  { x: 9912, y: 12120, z: 15 } ]
```
