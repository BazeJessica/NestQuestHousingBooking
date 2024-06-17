<template>
  <div class="propty">
    <img :src="property.image" alt="Property Image" class="property-image">
    <h3>
        {{property.title}}
    </h3>
    <p>{{property.type}} </p>
    <p style="color:rgb(194, 44, 44); font-style:bold;">{{property.amount}}</p>

     <p class="vectors">
        <span> {{property.vectors.roomNo}}</span>
         <span> {{property.vectors.Showers}}</span>
         <span>{{property.vectors.Ratings}} </span>
    </p>
    

</div>
</template>

<script>
export default {
  name: "PropertyComponent",
  props: {
    property: Object,
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,100..1000;1,9..40,100..1000&display=swap');

.propty {
  font-family: "DM Sans", sans-serif;
  font-optical-sizing: auto;
  font-weight: 4px;
  font-style:normal;
  border-radius: 15px; /* add border radius */
  box-sizing: border-box; /* add box-sizing */
  margin: 20px;
  padding: 20px; /* add padding */
  width: 100%; /* add width */
  box-shadow: 0px 0px 10px rgba(0,0,0,0.1); /* add box-shadow */
}

.property-image {
  border-radius: 10px 10px 0px 0px; /* add border radius */
  width: 100%; /* add width */
  height: auto; /* add height */
}

.vectors {
  color: rgb(22, 4, 4);
}

span {
  margin-right: 20px;
}

p {
  color: black;
}

h3 {
  color: black;
}
</style>