<template>
  <div class="container">
    <Home />
    <Properties :properties="properties"  />
  </div>
</template>

<script>
import Home from './components/Home.vue'
import Properties from "./components/Properties.vue";
export default {
  name: 'App',

  components: {
    Home,
    Properties
  },

  data(){
    return{
      properties:[]
    }
    
  },
  methods: {
    async fetchProperties(){
      const res = await fetch('http://localhost:5000/properties')

      const data = await res.json()

      return data

    }
  },

  async created(){
    
    this.properties = await this.fetchProperties()
  }
}
</script>



<style>
body{
  margin: 0;
  padding: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #faf9f9;
  margin: 40px auto; /* add some margin to create space around the app */
  padding: 20px; /* add some padding to create space inside the app */
  display: flex; /* use flexbox to align content vertically */
  flex-direction: column; /* stack elements vertically */
  align-items: center; /* center elements horizontally */

}

  
</style>