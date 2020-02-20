# Onli

## Challenge Junior Fullstack: SSR VUE.js

TL;DR Crie um servidor node.js com uma rota onde devera retornar uma página renderizada com vue-server-renderer

Existe um "super framework" muito utilizado pelas empresas chamado Nuxt.js. Ele basicamente a forma mais facil de desenvolver aplicações SSR. Mas para esse teste você apenas poderá consultar como ele funciona (hahaha). Dica https://github.com/nuxt/nuxt.js/blob/dev/packages/vue-renderer/src/renderers/ssr.js. Sim, você pode utilizar o codigo utilizado aqui, mas nao recomendamos. Há muitas dependencias e não precisamos de varias coisas que esse arquivo faz. Mais uma dica, use e abuse do vue-server-renderer. 

Tempo estimado do teste é de 1hr. 

Nesse desafio, iremos avaliar sua proeficiência, habilidade de pesquisa, utilização API de Bibiliotecas e leitura de código Open Source.

- render
  - onlicomponent.js
  - index.html
  - index.js
- boot.js 

render/onlicomponent.js
```javascript
  // define
  var OnliComponent = Vue.extend({
    template: '<div>A custom component!</div>'
  })
  // register
  Vue.component('onli-component', OnliComponent)
  // create a root instance
  new Vue({
    el: '#example'
  })
```

render/index.html:
```html
  <!-- index.html -->
  <html><body>
    <div id="example">
      <onli-component></onli-component>
    </div>
  </body></html>
```
