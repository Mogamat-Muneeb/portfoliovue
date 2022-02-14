<template>

 <div class="container">
    
<div class="row row1 d-flex justify-content-center">
    <h1 class="headin d-flex justify-content-center"><span  style="color:#FF7779;">About Me</span> </h1>
  <div class="box d-flex justify-content-center  col-sm-6 ">
      <img class="photo" src="https://i.postimg.cc/Y9PqgTJG/Muneeb-min.jpg" alt="" >
  </div>

  <div class=" col-sm-6">
  <h1 class="hi" style="color:#89CFF0;" >Hi Guys!</h1>
  <h6 class="h d-flex justify-content-start fw-bold" style="color: #FF7779;">Bio:</h6>
  <p> I am a person that works hard, trying my best to be punctual at my studies or anything that needs my full attention. I'm a person that is always willing to assist others when in need. I'm very comfortable around lots of people. I'm a confident and open person.</p>
  <h6  class=" heading fw-bold" style="color: #FF7779;">Where my passion for coding started:</h6>
  <p>My passion for the tech/coding industry started when I realized that technology is the future. I always wondered how websites and mobile applications were built that is the main reason I started looking into coding.</p>
 
  <div class="about-profile">   
<ul class="admin-profile">

<li><span class="pro-title"> D.O.B      </span> <span class="pro-detail">20/08/2001</span></li>
<li><span class="pro-title"> Country    </span> <span class="pro-detail">South Africa</span></li>
<li><span class="pro-title"> Location   </span> <span class="pro-detail">Cape Town</span></li>
<li><span class="pro-title"> e-mail     </span> <span class="pro-detail">davimuneeb785@gmail.com</span></li>
<li><span class="pro-title"> Phone      </span> <span class="pro-detail">+ (27) 76 162 1649</span></li>
<li><span class="pro-title"> Freelance  </span> <span class="pro-detail">Available</span></li>
</ul>
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
/* .bio{
    padding-right: 60px;
} */

h1{
    padding-top:110px;
}

.container {
    display:flex;
    flex-wrap: wrap;
    /* height:100vh; */
    /* position:fixed; */
    
   
}
.photo{

    
    height: 350px;
    width: 350px;
    object-fit:cover;
      box-shadow:8px 8px 15px #e4e4e4;
    margin-right: -100px;
    margin-top:120px; 
    /* border: 5px solid white; */
    border-radius:20px;
}

.hi{
    display: flex;
    justify-content: center;
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
    /* justify-content:space-between; */
    width:300px;
}
.about-profile .pro-title {
    font-weight: 700;
    color: #2c3e50;
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
    color: #89CFF0;
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
    /* margin-top:120px;  */
    /* border: 5px solid white; */
    /* border-radius:20px; */
}
}
/* 
@media only screen and (max-width: 1000px){
  .photo {
        height: 400px;
  }

  .row{
    text-align:none;
    
}
.about-profile{
    font-size:-15px ;
}
}

@media only screen and (max-width: 600px){
   .row{
    text-align:left !important;
   }
    .pro-title{
 
     margin-left:-95px;
    text-align:left !important;
}
}



@media only screen and (max-width: 720px){
   .row{
    text-align:left !important;
   }
    .pro-title{
 
     margin-left:-120px;
    text-align:left !important;
}
}


@media only screen and (max-width: 535px){
   .row{
    text-align:left !important;
   }
    .pro-title{
 
     margin-left: -160px;
    text-align:left !important;
}
.about-profile{
    margin-right:-50%;
}
} */
/* 
@media only screen and (max-width: 904px){
   .row{
    text-align:center !important;
    
   }
    .pro-title{
 
     margin-left: 10px;
    text-align:left !important;
}
.about-profile{
    margin-right:-145%;
}
.h{
    padding-left:110px;
} */


@media only screen and (max-width: 494px) {
    h1.headin{
    padding-top:50px;
}
}
</style>