# visual-debug

Quickly draw shapes on the viewport to visualise front-end problems.

# Installation

```
npm i visual-debug
```

# Usage

```javascript
import * as visualDebug from 'visual-debug'
```

To draw a rectangle:

```javascript
visualDebug.drawRect({
  x, // in pixels
  y, // in pixels
  width, // in pixels
  height, // in pixels
  color, // [Optional] Example: 'rgba(255, 255, 0, 1)'
  // If no color is provided, a random one is chosen
})
```

To draw a horizontal guide:

```javascript
visualDebug.drawGuideHorizontal({
  y, // in pixels
  color, // [Optional] Example: 'rgba(255, 255, 0, 1)'
  // If no color is provided, a random one is chosen
})
```

To draw a vertical guide:

```javascript
visualDebug.drawGuideVertical({
  x, // in pixels
  color, // [Optional] Example: 'rgba(255, 255, 0, 1)'
  // If no color is provided, a random one is chosen
})
```

To highlight a DOM element:

```javascript
visualDebug.highlightElement({
  selector, // standard CSS selector as a string
  color, // [Optional] Example: 'rgba(255, 255, 0, 1)'
  // If no color is provided, a random one is chosen
})
```

To clear everything:

```javascript
visualDebug.clear()
```
