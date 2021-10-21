<template>

<!-- Indecision component, segunda parte del proyecto -->
  <Indecision />



  <!-- Agregamos la prop title y definimos su valor aquí, generalemnte se usa kebab-case -->
  <!-- Enlazamos el numero con : a la prop del componente -->
  <!-- <Counter title="Entraron"
           :start="15" /> -->
           <!-- counter definido por defecto en el componente -->
           <!-- <Counter title="Entraron"
            /> -->
  <!-- <Counter title="Salieron" /> -->
</template>

<script>
//import Counter from './components/Counter.vue'
import Indecision from './components/Indecision.vue'

export default {
  name: 'App',
  components: {
    //Counter
    Indecision
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  
}
</style>
