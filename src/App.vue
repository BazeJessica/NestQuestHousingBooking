<template>
  <div>
    <Header />
    <Properties :properties="properties"  />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Properties from "./components/Properties.vue";
export default {
  name: 'App',

  components: {
    Header,
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
  color: #e5e5e5;
  margin: 50px auto;
  max-width: 1000px;
}

img {
  height: 40px;
}

h1 {
  text-align: center;
  font-size: 30px;
}
</style>