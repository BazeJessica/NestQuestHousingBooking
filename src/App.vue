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

  created(){
    this.properties=[
      {
        id:1,
        image:"./assets/istockphoto-1140134578-612x612.jpg",
        title:"2578 Folsom street, san francisco, CA, 94110",
        type:"Private  Room",
        amount:"$3200.00",
        vectors:{
          roomNo:"⛺4",
          Showers:"🛀shower",
          Ratings:"👍3",
        }

      },
      {
        id:2,
        image:"./assets/istockphoto-119854218-612x612.jpg",
        title:"2578 Folsom street, san francisco, CA, 94110",
        type:"Shared  Room",
        amount:"$2130.00",
        vectors:{
          roomNo:"⛺2",
          Showers:"🛀shower",
          Ratings:"👍 4",
        }

      },
      {
        id:3,
        image:"./assets/istockphoto-531345355-612x612.jpg",
       title:"2578 Folsom street, san francisco, CA, 94110",
       type:"Shared  Room",
        amount:"$4312.00",
        vectors:{
          roomNo:"⛺3",
          Showers:"🛀shower",
          Ratings:"👍 5",
        }

      },
      {
        id:4,
        image:"./assets/istockphoto-531345355-612x612.jpg",
       title:"2578 Folsom street, san francisco, CA, 94110",
       type:"Private  Room",
        amount:"$4312.00",
        vectors:{
          roomNo:"⛺2",
          Showers:"🛀shower",
          Ratings:"👍 4",
        }

      },
      {
        id:5,
        image:"./assets/istockphoto-531345355-612x612.jpg",
       title:"2578 Folsom street, san francisco, CA, 94110",
       type:"Private Room",
        amount:"$2312.00",
        vectors:{
          roomNo:"⛺5",
          Showers:"🛀shower",
          Ratings:"👍 2",
        }

      },
      {
        id:5,
        image:"./assets/istockphoto-531345355-612x612.jpg",
       title:"2578 Folsom street, san francisco, CA, 94110",
       type:"Shared  Room",
        amount:"$1212.00",
        vectors:{
          roomNo:"⛺3",
          Showers:"🛀shower",
          Ratings:"👍 5",
        }

      }
    
    ]
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