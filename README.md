# vue-svg-loader <img src="https://img.shields.io/npm/dt/vue-svg-loader.svg">
A webpack loader that allows to use SVG files as Vue Components.

## Installation
```
npm i vue-svg2-loader -D
```

## Configuration
```js
{
  test: /\.svg$/,
  loader: 'vue-svg2-loader', // `vue-svg` for webpack 1.x,
  options: {
      classes: 'default-class-1 default-class-2'
  }
}
```

## Example code

```html
<template>
  <nav id="menu">
    <a href="...">
      <SomeIcon class="icon" />
      Some page
    </a>
  </nav>
</template>

<script>
import SomeIcon from './assets/some-icon.svg';

export default {
  name: 'menu',
  components: {
    SomeIcon,
  },
};
</script>
```
---
*The idea behind this was inspired by [react-svg-loader](https://github.com/boopathi/react-svg-loader)*.
