// Définition d'un nouveau composant appelé `allProject`

Vue.component('allProject', {
  data: function () {
    return {
      count: 0
    }
  },
  template: '<button v-on:click="count++">Vous m\'avez cliqué {{ count }} fois.</button>'
})