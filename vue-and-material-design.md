### Vue and Material Design

some references:

[http://vuematerial.io](http://vuematerial.io/#/ "vuematerial.io")

[CodingTheSmartWay - Using Material Design with Vue.js 2](https://medium.com/codingthesmartway-com-blog/using-material-design-with-vue-js-2-a938eac53112)

[Vuetify.js](https://vuetifyjs.com/)

Let's build some basic web with Vue and material \( I'll call the project vmweb \)

```
// create the project using vue CLI and webpack
vue init webpack vmweb

// Get into the project and install packages
cd vmweb
npm install

// run it
npm run dev
```

Let's add vue-material library to the project

```
npm install --save vue-material
```

...and install font library and icon pack into index.html

```
<link href='https://fonts.googleapis.com/css?family=Roboto:300,400,500,700|Material+Icons' rel="stylesheet" type="text/css">
```

From CDN

[Javascript](https://unpkg.com/vue-material)

[CSS](https://unpkg.com/vue-material/dist/vue-material.css)

use the whole library

```
var Vue = require('vue')
var VueMaterial = require('vue-material')

Vue.use(VueMaterial)
```



[JSFiddle](https://jsfiddle.net/CruzJT/5j448rh7/3/)

