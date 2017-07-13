### Nested Components

By creating your own components your app could be much more semantic and understandable...

If  you write some code using &lt;ul&gt; and &lt;li&gt; tags someone who come later could be lost... if, instead, we write using tags like &lt;task-list&gt; and &lt;task&gt; that is much more easy to understand, right?

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

