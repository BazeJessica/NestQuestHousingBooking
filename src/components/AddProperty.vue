<template>
  <form class="add-form">
    <p>Your Property With Us And Be Confident That Your Room Will Be Filled Out!</p>
    <h2>Add A New Property</h2>
    <div class="form-grid">
      <div class="form-control">
        <label> Name </label>
        <input type="text" name="name" v-model="name" placeholder="Enter Name"> 
      </div>
      <div class="form-control">
        <label> Address </label>
        <input type="text" name="address" v-model="address" placeholder="Enter Address"> 
      </div>
      <div class="form-control">
        <label> Unit Number</label>
        <input type="text" name="Unit Number" v-model="unitNumber" placeholder="Enter Unit"> 
      </div>
      <div class="form-control">
        <label> City</label>
        <input type="text" name="City" v-model="city" placeholder="Enter City"> 
      </div>
      <div class="form-control">
        <label> State</label>
        <input type="text" name="State" v-model="State" placeholder="Enter State"> 
      </div>
      <div class="form-control">
        <label> Room Type </label>
        <select name="roomtype" v-model="roomType">
          <option value="SharedRoom" selected>
            Select a roomtype
          </option>
          <option value="SharedRoom">
            Shared Room
          </option>
          <option value="PrivateRoom">
            Private Room
          </option>
        </select>
      </div>
      <div class="form-control">
        <label> Price</label>
        <input type="text" name="price" v-model="price" placeholder="Enter Price"> 
      </div>
       </div>
      <div class="form-control">
        <label> Description</label>
        <textarea name="textAres" cols="100" rows="20" v-model="description">Enter Description</textarea>
      </div>
     
      <div class=" btn">
        <input type="submit" value="Add New Property">
      
    </div>
  </form>
</template>

<script>
export default {
  name: "AddProperty",
  data(){
    return{
      name: " ",
      address: " ",
      unitNumber: " ",
      State: " ",
      city: " ",
      price: " ",
      roomType: " ",
      description: " ",
    }
  }
}
</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

.add-form {
  margin-top: 100px;
  color: black;
  margin-left: 20px;
  margin-right: 20px;
  font-size: 18px;
  font-family: "Poppins", sans-serif;
  font-weight: 500;
  font-style: normal;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.4);
  padding: 25px;
  border: 1px solid #ccc;
  border-radius: 10px;
}
p{
    font-family: "Inter", sans-serif;
  font-optical-sizing: auto;
  font-style: normal;
  font-variation-settings:
    "slnt" 0;

}
.form-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 20px;
  
}

.form-control {
  margin: 20px 0;
}

.form-control label {
  display: block;
}

.form-control input,.form-control select {
  width: 100%;
  height: 60px;
  padding: 3px 7px;
  font-size: 17px;
  box-sizing: border-box;
  background-color: #F9F9F9;
}
/* .form-control input[placeholder]{
    color: black;

} */

.btn {
  display: block; /* to center the button */
  margin: 0 auto; /* to center the button */
  padding: 20px;
  width: 400px; /* set a fixed width */
  height: 40px; /* set a fixed height */
  background-color: #008000; /* set a green background color */
  color: #ffffff; /* set white text color */
  border: none; /* remove the default border */
  cursor: pointer; /* change the cursor to a pointer on hover */
  text-align: center; /* to horizontally center the text */
  font-size: 24px; /* increase the font size */
}

</style>