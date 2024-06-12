<template>

<div>
    <Button text="View All Property" color="red" class="btn"/>
    <h2>List of Properties</h2>
    <div class="property-grid">
        <div :key="property.id"  v-for="property in properties" class="proper-item">
        <Property :property="property" />
        </div>
    </div>
    
    <Button text="previous" color="#000" class="btn"/>
    <Button text="next" color="#000" class="btn"/>
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
h2{
    padding-top: 50px;
    padding-left: 20px;
}
div{
     margin: 30px auto;
     background-color: rgba(124, 123, 123, 0.5);
}
.btn {
    
  display: inline-block;
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
  float: right;

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
}
.property-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 20px;
}

.property-item {
  
  padding: 20px;
  border-radius: 30px;
 
}
</style>