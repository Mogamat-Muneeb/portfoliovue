<template>

 <div class="container">
    
<div class="row row1 d-flex justify-content-center">
    <h1 class="headin d-flex justify-content-center fw-bold"><span  style="color:#1e90ff;">About Me</span> </h1>
  <div class="box d-flex justify-content-center  col-sm-6 ">
      <img class="photo" src="https://i.postimg.cc/Y9PqgTJG/Muneeb-min.jpg" alt="" >
  </div>

  <div class=" col-sm-6">
  <h1 class="hi" style="color:#00bfff;" ></h1>
  <h6 class="h d-flex justify-content-start fw-bold" style="color: #1e90ff;"></h6>
  <p>Hi! I’m <span style="color: #00bfff;" class="fw-bold">Mogamat Muneeb Davids</span> , and I'm a developer who has a passion for building clean web applications with instinctive functionality. I enjoy turning ideas into reality via coding. I'm a hardworking and time-conscious person. I'm always willing to assist others when in need as well as being comfortable around people. I'm confident and am open to new ideas...</p>
  <p>My passion for technology and coding began when I realized that technology was the future. I have always wondered how Web applications and Mobile apps were built, which is why I decided to dig deeper into Web Development and Coding.</p>

  <div class="about-profile">   
    <ul class="admin-profile">

    <li><span class="pro-title" style="color:#1e90ff;"> D.O.B      </span> <span class="pro-detail">20/08/2001</span></li>
    <li><span class="pro-title" style="color:#1e90ff;"> Country    </span> <span class="pro-detail">South Africa</span></li>
    <li><span class="pro-title" style="color:#1e90ff;"> Location   </span> <span class="pro-detail">Cape Town</span></li>
    <li><span class="pro-title" style="color:#1e90ff;"> E-mail     </span> <span class="pro-detail">davimuneeb785@gmail.com</span></li>
    <li><span class="pro-title" style="color:#1e90ff;"> Phone      </span> <span class="pro-detail">+ (27) 76 162 1649</span></li>
    <li><span class="pro-title" style="color:#1e90ff;"> Freelance  </span> <span class="pro-detail">Available</span></li>
    </ul>
 </div>
 <div class="col d d-flex ">
      <div class="hire">
       <router-link :to="{ name: 'Contact'}"><button class="btn btn-mod btn-border btn-large">HIRE ME</button></router-link>
 </div>
 <div class="download">
      <button class="btn btn-mod btn-border btn-large"><a href="https://drive.google.com/file/d/1YIhBJGO8LqJHhIq_pEiUFy9YIm_DSWFn/view?usp=sharing" target="_blank">VIEW CV</a></button>
 </div>
 
 </div>


  </div>
</div>


</div>


</template>

<script>
export default {

}
</script>

<style scoped>
.d{
    margin-left: -13px;
}
a{
    text-decoration: none;
    color:white
}
a:hover{
    color: #012966;
}
.btn{
    margin-left: 10px;
}
.btn-mod.btn-large {
    height: auto;
    padding: 10px 52px;
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
    text-decoration: none !important;
    letter-spacing: 2px;
    -webkit-border-radius: 0;
    -moz-border-radius: 0;
    border-radius: 0;
    -webkit-box-shadow: none;
    -moz-box-shadow: none;
    box-shadow: none;
}

.btn-mod.btn-border:hover, .btn-mod.btn-border:active, .btn-mod.btn-border:focus, .btn-mod.btn-border:active:focus {
     color:  #012966;
    border-color:#9dd8e0 ;
    background:#9dd8e0;
    outline: none;
    
    
}
p{
    font-weight: 500;
}

h1{
    padding-top:110px;
}

.container {
    display:flex;
    flex-wrap: wrap;
  
    
   
}
.photo{

    
    height: 350px;
    width: 350px;
    object-fit:cover;
    box-shadow:8px 8px 15px #e4e4e4;
    margin-right: -100px;
    margin-top:70px; 
    border: 6px solid white;
    border-radius:50%;
}

.hi{
    display: flex;
   
    padding-top:50px;
}
.admin-profile{
    display: grid;
    justify-content: center;
    padding-left: 30px;
    padding-bottom: 40px;
}
.row{
    text-align:left ;
    margin-top:15px;
    margin-bottom:15%;
}


 .about-profile .pro-detail{
    text-align:center !important;
    
}
.about-profile li{
    display: flex;
    
    width:300px;
}
.about-profile .pro-title {
    font-weight: 700;
    /* color: #2c3e50; */
    position: relative;
    width: 120px;
    display: inline-block;
    margin-bottom: 5px;
    
}

.pro-title{
    margin-left: -183px;
}

.about-profile .pro-title:after {
    position: absolute;
    content: ':';
    color: #00bfff;
    font-size: 14px;
    left: 100px;
   
}

ul li, ol li {
    list-style: none;
}


@media screen and (max-width: 494px){
    .photo{

    
    height: 270px;
    width: 270px;
    object-fit:cover;
    box-shadow:8px 8px 15px #e4e4e4;
    margin-right: auto;
    margin-left: auto;
   
}
}

@media only screen and (max-width: 494px) {
    h1.headin{
    padding-top:50px;
}


.pro-title{
    margin-left: -65px;
}

}

@media only screen and (max-width: 494px) {
 .btn{
    margin-left: 2px;
}
.btn-mod.btn-large {
    height: auto;
    padding: 15px 30px;
    font-size: 11px;
    border-radius: 30px;
}

.btn-mod.btn-border {
    color: #fff;
    border: 1px solid #1e90ff;
    background: #1e90ff;
}

.btn-mod, a.btn-mod {
    /* -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box; */
    /* padding: 4px 13px; */
    /* color: #fff; */
    /* background: rgba(34,34,34, .9); */
    border: 1px solid transparent;
    font-size: 11px;
    font-weight: 400;
    /* text-transform: uppercase; */
    text-decoration: none !important;
    letter-spacing: 0.3px;
    -webkit-border-radius: 0;
    -moz-border-radius: 0;
    border-radius: 0;
    -webkit-box-shadow: none;
    -moz-box-shadow: none;
    box-shadow: none;
}


}

</style>