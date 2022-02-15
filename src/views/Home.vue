<template>
  <div class="container">
    <div class="row">
      <div class="name col">
        <h6 style="font-size: 15px;color: #00bfff;">HEY! I AM</h6>
        <h1  style="font-size:60px;">M.Muneeb Davids !</h1>
        <!-- <h1 class="type" style="color:#FF7779;">An Aspiring Full Stack Developer</h1> -->
        <h1  style="color:;font-size:20px;">An Aspiring <span class="blink">
  <span class="blink-hard" style="color:#1e90ff;font-size:20px;">Full Stack Developer</span>
    
  </span> </h1>
      </div>
      <div class="col">
        <img src="https://i.postimg.cc/Y2sZ1ZNp/IMG-20210815-WA0040-removebg-preview.png" alt="">
      </div>
    </div>
  </div>
</template>

<script>
export default {
 

      
}

 
        
</script>

<style scoped>
/* .blink {

   display:flex;
  justify-content: center;
  flex-direction: column;
  
 
} */

.blink-hard {
  animation: pulse 4s infinite;
}

@keyframes pulse {
  50% {
    opacity: 0;
  }
}

.container {
   /* height:100vh; */
  padding-top: 150px;
  margin-bottom:50px;
 
}
/* .row{
    display: flex;
  flex-wrap:wrap;
} */
.name{
  padding-top:135px;
  padding-left: 135px;
}
img{
  height:450px;
  object-fit: cover;
  padding-right: 130px;
  
}
h6{
  font-weight: 700;
}
h1{
  font-weight:700;
}
@media screen and (max-width: 494px){
.name{
  padding-top:10px;
  padding-left:10px;
}
img{
  height:250px;
  object-fit: cover;
  padding-right: 130px;
  padding-left:130px;
}
.container {
   height:80vh;
   
  /* padding-top: 150px; */
 
}
.row {
  overflow-x: hidden;
}
}

</style>