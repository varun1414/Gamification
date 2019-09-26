<template>
     <div>
       <link href='https://fonts.googleapis.com/css?family=Clicker Script' rel='stylesheet'>
       <ul>
  <li><a class="active" @click="about()">About</a></li>
  <li><a @click="login()">Order Food!</a></li>
  </ul>
   <q-carousel
      style="padding-top:1px"
      animated
      v-model="slide"
      arrows
      navigation
      infinite
    >
      <q-carousel-slide :name="1" img-src="https://i0.wp.com/vegecravings.com/wp-content/uploads/2017/04/paneer-butter-masala-recipe-step-by-step-instructions.jpg?fit=2592%2C1944&ssl=1"/>
      <q-carousel-slide :name="2" img-src="https://media.istockphoto.com/photos/indian-food-selection-picture-id153775715?k=6&m=153775715&s=612x612&w=0&h=ifR9QGS-yfFRdpNgAoWjue3iBYdzrkMBDgWR25Rh8Rg=" />
      <q-carousel-slide :name="3" img-src="http://www.hungerfree.in/adminupload/gopi-65.jpg" />
      <q-carousel-slide :name="4" img-src="https://i1.wp.com/files.hungryforever.com/wp-content/uploads/2015/07/18115007/veg-kadai-recipe.jpg?resize=1075%2C605&ssl=1" />
    </q-carousel>
    <div style="background-color:	#DCDCDC; padding-top: 23px; padding-bottom:1px">
      <h4 align="center" class="font"><strong>FoodIt</strong></h4>
    </div>
    </div>
  </template>
  <script>
   export default {
     data(){
       return{
          slide: 1
       }
     },
     methods:
     {
       login(){
         this.$router.push('/login')
       },
       about(){
         this.$router.push('/about')
       }
       
     }
   }
   </script>
     <style>
     .font{
        font-family: 'Clicker Script';font-size: 75px;
     }
        ul {
  list-style-type: none;
  margin: 0;
  padding: 3px;
  overflow: hidden;
  background-color:orange;
}

li {
  float: right;
}

li a {
  font-family: 'Clicker Script';
  font-size: 22px;
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

li a:hover {
  background-color: green;
}
     
     h1{
       position: relative;
       left: 450px;
       
       font-family: 'Sofia';
       font-size: 50px;
     }
     </style>
       
      
    
  
    