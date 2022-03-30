<template>
  <div class="container">
    <div class="row">
      <div class="name col">
        <h6 style="font-size: 15px;color: #00bfff;">HEY! I AM</h6>
        <h1  style="font-size:60px;">M.Muneeb Davids !</h1>
     
        <h1  style="color:;font-size:20px;">An Aspiring <span class="blink">
  <span class="blink-hard" style="color:#1e90ff;font-size:20px;">Full Stack Developer</span>
    
  </span> </h1>
      </div>
      <div class="col">
        <img src="https://i.postimg.cc/z5N3Nhgh/Whats-App-Image-2022-02-18-at-10-22-51-AM.jpg" alt="">
      </div>
    </div>
  </div>
</template>

<script>
export default {
 

      
}

 
        
</script>

<style scoped>


.blink-hard { 
  animation: pulse 4s infinite;
}


@keyframes pulse {
  50% {
    opacity: 0;
  }
}
/* .btn-mod.btn-large {
    height: auto;
    padding: 13px 52px;
    font-size: 15px;
    border-radius: 30px;
}

.btn-mod.btn-border {
    color: #fff;
    border: 1px solid #1e90ff;
    background: #1e90ff;
}

.btn-mod, a.btn-mod {
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
    padding: 4px 13px;
    color: #fff;
    background: rgba(34,34,34, .9);
    border: 1px solid transparent;
    font-size: 11px;
    font-weight: 400;
    text-transform: uppercase;
    text-decoration: none;
    letter-spacing: 2px;
    -webkit-border-radius: 0;
    -moz-border-radius: 0;
    border-radius: 0;
    -webkit-box-shadow: none;
    -moz-box-shadow: none;
    box-shadow: none;
    -webkit-transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
    -moz-transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
    -o-transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
    -ms-transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
    transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
}

.btn-mod.btn-border:hover, .btn-mod.btn-border:active, .btn-mod.btn-border:focus, .btn-mod.btn-border:active:focus {
    color: white;
    border-color:#9dd8e0 ;
    background:#9dd8e0;
    outline: none;
    
} */

.container {
   height:100vh;
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
  height:550px;
  object-fit: cover;
  
  
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
  height:450px;
  object-fit: cover;
  padding-top: 30px;
  /* padding-right: 130px; */
  /* padding-left:58px; */
  
}
.container {
   height:90vh;
   
  /* padding-top: 150px; */
 
}
.row {
  overflow-x: hidden;
}
}

</style>