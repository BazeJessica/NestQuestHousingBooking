<template>
<div class="propty">
    <img :src="property.image" alt="Property Image" class="property-image">
    <h3>
        {{property.title}}
    </h3>
    <p>{{property.type}} </p>
    <p style="color:rgb(194, 44, 44);">{{property.amount}}</p>

     <p class="vectors">
        <span> {{property.vectors.roomNo}}</span>
         <span> {{property.vectors.Showers}}</span>
         <span>{{property.vectors.Ratings}} </span>
    </p>
    

</div>
    
</template>

<script>


export default{
   name: "PropertyComponent",
   
   props:{
    property:Object,

   }

}
</script>

<style scoped>
.vectors{
    color: rgb(22, 4, 4);
}
span{
    
    margin-right: 20px;

}
.propty{
    border-radius: 30px;
    display: inline-block;
    margin: 5px;
    padding: 10px 20px;
    cursor: pointer;
}
.propty.reminder{
    border-left:5px solid green;
}
.propty h3{
    display: flex;
    align-items: center;
    justify-content: space-between;
    }

</style>