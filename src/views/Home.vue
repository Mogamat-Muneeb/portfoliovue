<template>
  <div class="container">
    <div class="row">
      <div class="name col">
        <h6 style="font-size: 15px;color: #89CFF0;">HEY! I AM</h6>
        <h1  style="font-size:60px;">M.Muneeb Davids !</h1>
        <!-- <h1 class="type" style="color:#FF7779;">An Aspiring Full Stack Developer</h1> -->
        <h1  style="color:;font-size:20px;">An Aspiring<span class="type">
  <span  style="color:#FF7779;font-size:20px;">Full Stack Developer</span>
    
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


.type {
  display: inline-flex;
}

.type span {
  word-break: break-all;
  height: 1em;
  width: 0%;
  overflow: hidden;
  animation: t 4s linear infinite alternate;
}
.type span:before {
  content: " ";
  display: inline-block;
}

@keyframes t {
  90%,
  100% {
    width: 100%;
  }
}




.container {
   /* height:100vh; */
  padding-top: 150px;
 
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
</style>