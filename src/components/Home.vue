<template>
  <header>
    <Nav />
    <hr/>
   <h1>The Most Affortable
      <br>
      Place To Stay In The
       <br>
      San Franciso Bay Area</h1>
  </header>
</template>

<script>
import Nav from "./Nav.vue"

export default {
  name: "HomeComponent",
  components: {
    Nav,
  }
};
</script>

<style >

@import url('https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,100..1000;1,9..40,100..1000&family=Inter:wght@100..900&display=swap');

header {
   margin-left: 20px;
   margin-right: 20px;
  background-image: url("https://wallpapercave.com/wp/wp7113919.jpg");
  background-size: cover;
  height: 70vh;
  background-color: rgb(0,0,0,0.5);
  filter: brightness(0.9); /* adjust the brightness level (0.8 is 80% of the original brightness) */
  color: #f1efef;
  display: flex; /* add flexbox to center content */
  flex-direction: column; /* stack elements vertically */
  padding: 10px;}


.logo {
  display:flex;
  align-items: center;
  /* margin-right: 20px; */
}

.logo img {
  height: 80px;
  justify-content: space-between;
  /* margin-right: 10px; */
}


nav a {
  text-decoration: none;
  margin-right: 50px; 
  color: #e5e5e5;
}

nav a:hover {
  color: #fff;
  text-decoration: underline;
  text-underline-offset: 15px; /* add this property to create a gap between the text and the underline */
}

h1{
  margin-top: 100px;
  margin-left: 100px;
  font-family: "Inter", sans-serif;
  font-optical-sizing: auto;
  color: #fff;
  font-style: normal;
  font-variation-settings: "slnt" 0;
  line-height: 1.2; /* add this to increase the space between rows */
  word-spacing: 0.3em; /* add this to increase the space between words */
}

/* hr{
  margin: 20px auto; ;
} */
</style>