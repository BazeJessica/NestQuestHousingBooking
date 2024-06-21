<template>
    <div class="logo">
      <div>
        <img alt="Housing logo" src="/assets/file.png" />
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


nav{
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
    height: 80px;
    margin-left: 80px;

}

</style>