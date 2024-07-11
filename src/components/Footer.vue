<template>
        <footer>
            
             <hr/>
             <div class="logoTest">
                <img alt="Housing logo" src="https://th.bing.com/th/id/OIP.Rq-5VJotaBDf4pfn3pJZBQHaF7?w=200&h=180&c=7&r=0&o=5&pid=1.7" />
            <aside>
                <p>    345 Faulconer Drive, Suite 4 • Charlottesville, CA, 12345</p>
                <p> (123) 456-7890         <span>(123) 456-7890 </span>  </p>
            </aside>
               
            </div>
            
            <div class="base">
                    <a href="#">ABOUT US</a>
                    <a href="#">CONTACT US</a>
                    <a href="#">HELP</a>
                    <a href="#">PRIVACY POLICY</a>
                    <a href="#">DISCLAIMER</a>
                
                <p>Copyright @ 2020 Minimunlivingcost. All rights reserved</p>

            </div>
            
        </footer>

  
</template>

<script>


export default{
    name:'FooterComponent',
}
</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Assistant:wght@200..800&display=swap');

footer{
     padding-top:100px;
}

.base{
   
    font-family: "DM Sans", sans-serif;
    font-optical-sizing: auto;
    font-size: 17px;
    font-style:normal;
    display: flex; /* add flexbox to align nav items */
    justify-content: space-between; /* space out nav items */
    align-items: center; /* center nav items vertically */
     margin-top: 50px; /* adjust margin to create space between nav and logo */

}

.base a{
    text-decoration: none;
    color: black;

}
img{
    height:500px;
    margin-right: 250px;
}

.logoTest{
    font-family: "Assistant", sans-serif;
  font-optical-sizing: auto;
  font-weight: 17px;
  font-style: normal; 
  font-optical-sizing: auto;
    font-size: 24px;
    font-style:normal;
    display: flex; /* add flexbox to align nav items */
     /* space out nav items */
    align-items: center; /* center nav items vertically */
     margin-top: 50px; 
     padding-left: 60px;

}
</style>