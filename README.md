# Slider

Slider component for Vue Bulma.


## Installation

```
$ npm install vue-bulma-slider --save
```


## Examples

```vue
<template>
  <div>
    <slider type="success" size="large" :value="value" :max="100" :step="1" is-fullwidth @change="update"></slider>
    <input class="input" type="number" v-model="value" min="0" max="100" number>
  </div>
</template>

<script>
import Slider from 'vue-bulma-slider'

export default {
  components: {
    Slider
  },

  data () {
    return {
      value: 23
    }
  },

  computed: {
    per () {
      return this.value + '%'
    }
  },

  methods: {
    update (val) {
      this.value = Number(val)
    }
  }

 }
</script>
```


## Badges

![](https://img.shields.io/badge/license-MIT-blue.svg)
![](https://img.shields.io/badge/status-stable-green.svg)

---

> [fundon.me](https://fundon.me) &nbsp;&middot;&nbsp;
> GitHub [@fundon](https://github.com/fundon) &nbsp;&middot;&nbsp;
> Twitter [@_fundon](https://twitter.com/_fundon)
