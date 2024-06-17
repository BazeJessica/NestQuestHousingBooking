<template>
  <div>
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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #faf9f9;
  margin: auto 30px;
  /* max-width: 2000px; */
  
}


</style>