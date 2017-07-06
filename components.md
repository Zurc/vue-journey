### Nested Components

By creating your own components your app could be much more semantic and understandable...

Let's see an example:

```
Vue.component('task-list', {
  // wrapped in a single root element (the div)
  template: '<div><task v-for="item in tasks">{{ item.task }}</task>></div>,

  data() {
    return {
      tasks: [
        { task: 'Go to the store', complete: true },
        { task: 'Go to the email', complete: false },
        { task: 'Go to the farm', complete: true },
        { task: 'Go to the work', complete: false }
      ]
    };
  }
)};

Vue.component('task', {
  template: '<li><slot></slot></li>'
});

new Vue({
  el:'#root',
});
```

[JSFiddle](https://jsfiddle.net/CruzJT/uyL0kxvm/2/)





