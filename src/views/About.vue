<template>

 <div class="container">
    
<div class="row row1 d-flex justify-content-center">
    <h1 class="headin d-flex justify-content-center"><span  style="color:#1e90ff;">About Me</span> </h1>
  <div class="box d-flex justify-content-center  col-sm-6 ">
      <img class="photo" src="https://i.postimg.cc/Y9PqgTJG/Muneeb-min.jpg" alt="" >
  </div>

  <div class=" col-sm-6">
  <h1 class="hi" style="color:#00bfff;" >Hi Guys!</h1>
  <h6 class="h d-flex justify-content-start fw-bold" style="color: #1e90ff;">Bio:</h6>
  <p>I am hardworking and time conscious of anything that requires my attention. I'm always willing to assist others when in need. I'm very comfortable around lots of people. I'm confident and open-minded.</p>
  <p>My passion for technology and coding began when I realised that technology was the future. I have always wondered how web applications and mobile apps are built, which is why I decided to study coding.</p>

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
    border: 4px solid white;
    border-radius:50%;
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
    /* margin-top:120px;  */
    /* border: 5px solid white; */
    /* border-radius:20px; */
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
</style>