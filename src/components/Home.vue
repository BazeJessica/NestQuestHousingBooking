<template>
  <header>
    <div class="logo">
      <img alt="Housing logo" src="../assets/file (1).png" />
      <h4 style=" margin-left: 30px; margin-top:0%; font-size: 18px">
        NestQuest <br />
        <span style="font-size: 13px; margin-left: 20px">Housing</span>
      </h4>
    </div>

      <a href="#">Home</a>
      <a href="#">Landlord</a>
      <a href="#">Tenants</a>
      <a href="#">Contact Us</a>
    
    
  </header>
</template>

<script>
export default {
  name: "HomeComponent",
  
};
</script>

<style scoped>
header {
    margin-top: 20px;
  display: inline-flex;
}
a {
  color: #e5e5e5;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  margin-right: 25px;
  margin-left: 20px;
}
.logo {
  margin-right: 350px;
}

</style>