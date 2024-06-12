<template>
  <header>
    <div class="logo">
      <div>
        <img alt="Housing logo" src="../assets/file (1).png" />
       <h4 style="margin-left: 30px; margin-top: 0%; font-size: 18px">
        NestQuest <br />
        <span style="font-size: 13px; margin-left: 20px">Housing</span>
      </h4>
      </div>
      
   
    <nav>
      <a href="#">Home</a>
      <a href="#">Landlord</a>
      <a href="#">Tenants</a>
      <a href="#">Contact Us</a>
    </nav>
   </div>
   <h1>Find Your Home Away From Home
      <br> AND <br>
      Discover Comfort Anywhere</h1>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
};
</script>

<style scoped>
header {
 
  background-image: url("../assets/istockphoto-1140134578-612x612.jpg");
  background-size: cover;
  height: 70vh;
  align-items: center;
  padding: 20px;
  color: #e5e5e5;
  background-color: rgba(0, 0, 0, 0.5);
}
nav{
  margin-left: 300px;
  margin-top: -60px;
   /* display: flex; */
   align-items: center;
   width: 100%;
}

.logo {
  display:flex;
  align-items: center;
  margin-right: 20px;
}

.logo img {
  height: 40px;
  margin-right: 10px;
}


nav a {
  text-decoration: none;
  margin-right: 25px;
  color: #e5e5e5;
}

nav a:hover {
  color: #fff;
}
h1{
  margin-top: 70px;
}
</style>