<template>
<div>
  <Home />
  <h1> Find Your Home Away From Home
             <br>  AND  <br>
        Discover Comfort Anywhere</h1>
</div>
  
</template>

<script>
import Home from './components/Home.vue'
export default {
  name: 'App',
  components: {
    Home,
  },
      
}
</script>

<style>
#app { 
 font-family: Avenir, Helvetica, Arial, sans-serif;
-webkit-font-smoothing: antialiased;
-moz-osx-font-smoothing: grayscale;
color: #e5e5e5;
margin: 50px auto; /* Change this to center the element horizontally */
background-image: url("./assets/istockphoto-1140134578-612x612.jpg");
background-size: cover;
height: 70vh;
background-repeat: no-repeat;
/* display: flex; */
align-items: center;
justify-content: center;
max-width: 1000px;
background-color: rgba(0, 0, 0, 0.5);
background-blend-mode: multiply;
}

img{
  height: 40px;
}
h1{
  text-align: center;
  font-size: 30px;
}

</style>
