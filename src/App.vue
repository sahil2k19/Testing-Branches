<template>
  <h1>{{title }}</h1>
  <br>
  <div v-if="showModal"> 
    <Modal :header="header" :text="text" theme="sale"/>
  </div>
  <button @click="toggleModal"> open modal</button>
</template>

<script>
import Modal from "./components/Modal.vue"

export default {
  name: 'App',
  components:{Modal}, 
  data(){
    return {
      title:"My first Vue App",
      header: "Sign up for the GiveAway",
      text: "Grab your ninja swag for half Price",
      showModal:false
    }
  },
  methods:{
    toggleModal(){
      this.showModal= !this.showModal
    }
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
  margin-top: 60px;
}
</style>
