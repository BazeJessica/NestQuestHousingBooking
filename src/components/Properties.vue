<template>

<div class="container">
    <Button text="View All Property" color="red" class="btn"/>
    <h2>List of Properties</h2>
    <div class="property-grid">
        <div :key="property.id"  v-for="property in properties" class="proper-item">
        <Property :property="property" />
        </div>
   
    
    <Button text="previous" color="#000" class="btn"/>
    <Button text="next" color="#000" class="btn"/>

  </div>
    
</div>

    
</template>

<script>
import Button from "./Button" 
import Property from "./property"

export default {
    name: "PropertiesComponent",
    components:{
        Button,
        Property,
    },

    props:{
        properties: Array

    }
}
</script>

<style scoped>
.container{
 background-color: #F5F5F5;
 background-size: cover;
}
h2 {
  padding-top: 100px;
  padding-left: 50px;
  font-size: 30px;
  color: #000000;
  box-sizing: border-box; /* add this property */
}

div {
  margin: 20px;
  /* background-color: #F5F5F5; */
  box-sizing: border-box; /* add this property */
}

.btn {
  display: inline-block;
  color: #fff;
  background-color: #F4511E;
  border: none;
  padding:20px;
  margin: 30px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
  float: right;
  box-sizing: border-box; /* add this property */
}

.btn:focus {
  outline: none;
}

.btn:active {
  transform: scale(0.98);
}

.btn-block {
  display: block;
  width: 100%;
  box-sizing: border-box; /* add this property */
}

.property-grid {
  margin: 20px;
  /* background-color: #FFFFFF; */
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 2px;
  box-sizing: border-box; /* add this property */
}

.property-item {
  padding: 10px; 
  box-sizing: border-box; /* add this property */
}
</style>
}
