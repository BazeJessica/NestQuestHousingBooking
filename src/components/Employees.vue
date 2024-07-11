<template>
    <div class="videoSect">
        <div class="image-peek">
        <img src="/assets/Double quote.png/" alt="Quots" >
        <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam interdum nisl et nunc facilisis, a commodo eros mollis. Nunc vel pellentesque est. Curabitur at odio sit amet libero vulputate efficitur ac nec justo. Nulla vitae mauris quam. Nulla quam massa, faucibus id pretium ac, mattis eu velit. Donec sed risus a lacus fringilla finibus.
         Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam interdum nisl et nunc facilisis, a commodo eros mollis. Nunc vel pellentesque est. Curabitur at odio sit amet libero vulputate efficitur ac nec justo. Nulla vitae mauris quam. Nulla quam massa, faucibus id pretium ac, mattis eu velit. Donec sed risus a lacus fringilla finibus.
        </p>
        </div>
        
        <div class="iframe">
        <iframe width="780" height="638" src="https://www.youtube.com/embed/TuyZN5u4Dqw" title="100 New Modern Living Room TV Wall Designs I Inspirational Ideas" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
         </div>
    </div>
</template>


<script>

export default {
    name:"EmployeeComponent"
    
}
</script>

<style scoped>
.videoSect{
    display: inline-flex;
    margin: 20px;
    margin-top: 100px;
     background-color: #eee9e8;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.3);
}
p{
   padding: 40px;
   padding-right: 40px;
  
}
.image-peek {
  position: relative;
}

/* .image-peek img {
  position: absolute;
  top: 0;
  left: 0;
  /* width: 100%;
  height: 100%; */
  /* object-fit: cover;
  clip-path: polygon(0 0, 100% 0, 100% 20%, 0 20%);
}
*/
.image-peek p {
  position: relative;
  z-index: 1;
  font-size: 32px;
  
} 
.image-peek img{
    padding-top:40px ;
    padding-left: 30px;
    height: 40px;
    position: absolute;
}
</style>