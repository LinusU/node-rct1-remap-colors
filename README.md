# RCT1 Remap Colors

Remap colors that where used in the game RollerCoaster Tycoon 1.

## Installation

```sh
npm install --save rct1-remap-colors
```

## Usage

```javascript
var remapColors = require('rct1-remap-colors')

console.log('rgb(' + remapColors[8].displayColor + ')') // rgb(81,132,10)
```

## API

### `remapColors[idx]`

Get the remap color with index `idx`. Valid indexes is `0` through `31`
inclusively.

### `remapColor.displayColor`

Get the color that is displayed in the user interface when selecting this color.

### `remapColor.colors[idx]`

Get the color that should replace another color at index `idx`. Valid indexes is
`0` through `11` inclusively.

## Color format

All colors are exported as `[ red, green, blue ]` with the colors being
integers between `0` and `255` inclusively.
