### Practical Components

[Laracasts - learn Vue2 step by step](https://laracasts.com/series/learn-vue-2-step-by-step/episodes/9?autoplay=true)    episode 9

[https://alligator.io/vuejs/roundup-desktop-components/](https://alligator.io/vuejs/roundup-desktop-components/)    Desktop Webapp component libraries

---

As far as I know there is two totally different ways to create a component

The original way:

```
Vue.component('component-name', {
    template: ...
    data: ...
    ...
}
```

...and by using vue-loader as a \*.vue file...

```
<template>
  <div class="example">{{ msg }}</div>
</template>

<script>
export default {
  data () {
    return {
      msg: 'Hello world!'
    }
  }
}
</script>

<style>
.example {
  color: red;
}
</style>
```

[https://vue-loader.vuejs.org/en/start/spec.html](https://vue-loader.vuejs.org/en/start/spec.html)



ERRORS and solution

[struggling loading vue-material components](https://forum.vuejs.org/t/struggling-loading-vue-material-components-the-first-time/11018/2)

[Unknown custom element](https://forum-archive.vuejs.org/topic/2036/component-inside-component-unknown-custom-element-error-vueify/4)



