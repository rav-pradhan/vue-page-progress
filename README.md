# vue-page-progress

A simple component that provides a vertical or horizontal bar to track scroll progress for a given page.

Scroll progress can either be for horizontal or vertical scrolling.

## Installation

```shell
npm i vue-page-progress
```

## Usage

### Global Registration
```vue
// main.js
import VuePageProgress from 'vue-page-progress'

Vue.component('VuePageProgress', VuePageProgress)
```

```vue
// in your component
<template>
  <div>
    <VuePageProgress />
  </div>
</template>
```

### Or Register And Use In A Component 
```vue
<template>
  <div>
    <VuePageProgress />
  </div>
</template>

<script>
import VuePageProgress from "vue-page-progress";
export default {
  name: 'app',
  components: {
    VuePageProgress
  }
}
</script>
```

### Props (all optional)

| Property | Type   | Default | Prop Description                       |
|----------|--------|---------------|-----------------------------------|
| meterSize  | String | 3px           |The size of the progress bar fill       |
| colour   | String | #61E2CF       | The colour of the progress bar fill |
| scrollDirection | String | "vertical"   | Corresponds to whether or not the scroll progress meter should fill based on `horizontal` or `vertical` scrolling         |
| barPosition  | String | "top"        | The position of the progress bar - can be either `top`, `right`, `bottom` or `left`   |
