<template>
  <div>
    <h2>{{  title }}</h2>
    <p>{{ counter }} <sup>2</sup> = {{ squareValue }}</p>

    <div>
      <button @click="increase">+1</button>
      <button @click="decrease">-1</button>
    </div>

  </div>
</template>

<script>
export default {
  // definimos la prop title y la llamamos dinamicamente en el template
    //props: ['title'],
    props: {
      title: String,
      //start: Number
      start: {
        type: Number,
        //valor definido por defecto desde el componente
        default: 1
      }
    },
    name: 'Counter',
    data() {
      return {
        //counter: 5
        counter: this.start
      }
    },
    methods: {
      getSquare() {
        return 'Hola Mundo'
      },
      increase(){
         //this.counter = this.counter +1
         this.counter++
      },
      decrease(){
        this.counter--
      }
    },
    computed: {
      squareValue() {
        console.log('Propiedad computada');
        return this.counter * this.counter
      }
    },
    
}
</script>

<style>
  button {
    margin:  0 5px;
    border-radius: 5px
  }
  button:hover{
    color: white;
    background-color: #42b883;
    cursor: pointer;
  }
</style>