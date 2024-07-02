<template>
    <div class="logo">
      <div>
        <img alt="Housing logo" src="https://th.bing.com/th/id/OIP.Rq-5VJotaBDf4pfn3pJZBQHaF7?w=200&h=180&c=7&r=0&o=5&pid=1.7" />
      </div>
      
        <nav>
            <a href="#">Home</a>
            <a href="#">Landlord</a>
            <a href="#">Tenants</a>
            <a href="#">Contact Us</a>
        </nav>
    
    </div>
</template>

<script>


export default {
    name:"NavComponent",
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,100..1000;1,9..40,100..1000&display=swap');

/* logo{
    margin-top: 20px;
} */
nav{
    padding-top: 40px;
    margin-left: 500px;
    font-family: "DM Sans", sans-serif;
    font-optical-sizing: auto;
    font-weight: 24px;
    font-size: 24px;
    font-style:normal;
    display: flex; /* add flexbox to align nav items */
    justify-content: space-between; /* space out nav items */
    align-items: center; /* center nav items vertically */
     margin-top: 2px; /* adjust margin to create space between nav and logo */

}

img{
    padding-top: 40px;
    margin-left: 80px;

}

</style>