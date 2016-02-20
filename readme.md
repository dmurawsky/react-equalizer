![Build Status](https://api.travis-ci.org/patrickgalbraith/react-equalizer.svg)

# React Equalizer

Pure React component which equalizes heights of child components.

### Installation

```
npm install --save react-equalizer
```

### Running Tests

Grab the latest source and in the project directory run:

```
npm install
npm test
```

### Usage

```jsx
<Equalizer>
  <div>Child 1</div>
  <div>Child 2</div>
  <div>Child 3</div>
</Equalizer>
```

With advanced options:

```jsx
<Equalizer
  byRow={false}
  property="maxHeight"
  enabled={(node) => window.matchMedia("(min-width: 400px)").matches}>
  <div>Child 1</div>
  <div>Child 2</div>
  <div>Child 3</div>
</Equalizer>
```

### Roadmap

* Add support for setting height of component based on total height of children

### References
* Zurb Foundation Equalizer
* jQuery Match Height
