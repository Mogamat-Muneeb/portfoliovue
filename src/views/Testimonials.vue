<template>
   <h1 class="headin d-flex justify-content-center"><span  style="color:#FF7779;">Testimonials</span> </h1>
   <div class="container">
       <div v-for="testimonial in testimonials" :key="testimonial" class="row">
  <div class="content">
    
      <div class="content-overlay"></div>
      <img class="content-image" :src="testimonial.img">
      <div class="content-details fadeIn-bottom">
        <h3 class="content-title">{{testimonial.title}}</h3>
        <h5 class="content-text">{{testimonial.relation}}</h5>
         <p class="content-text">{{testimonial.quote}}</p>
         <h6>{{testimonial.email}}</h6>
      </div>
    
  </div>

       </div>
   </div>
</template>

<script>
export default {
    data(){
    return {
      testimonials:[]
    }
  },
 
        mounted(){
            fetch('  https://myport-backend.herokuapp.com/testimonials')
            .then(res => res.json())
            .then(data => this.testimonials = data)
            .catch(err => console.log(err.message))
        }
}
</script>

<style scoped>

h1.headin{
    padding-top:110px;
}

/* .image img{
    width:300px;
    border-radius:10px;
}


.image img:hover{
    background:red;
} */


.container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;

}
/* 
.image {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  width: 300px;
  height: 300px;
  border-radius: 10px;
   box-shadow:8px 8px 8px #e4e4e4;
   margin: 10px;
} */


/* *, *:before, *:after{
  margin: 0;
  padding: 0;
  -webkit-box-sizing: border-box;
  -moz-box-sizing:border-box;
  box-sizing: border-box;
} */

/* body{
  background: #f9f9f9;
  font-size: 16px;
  font-family: 'Raleway', sans-serif;
} */

.main-title{
  color: #2d2d2d;
  text-align: center;
  text-transform: capitalize;
  padding: 0.7em 0;
}

/* .container{
  padding: 1em 0;
  float: left;
  width: 100%;
} */
/* @media screen and (max-width: 640px){
  .container{
    display: block;
    width: 100%;
  }
} */
/* 
@media screen and (min-width: 900px){
  .container{
    width: 33.33333%;
  }
} */

.container .title{
  color: #1a1a1a;
  text-align: center;
  margin-bottom: 10px;
}

.content {
 
  position: relative;
  width: 90%;
  max-width: 400px;
  margin: 10px;
  /* overflow: hidden; */
}

.content .content-overlay {
  /* background: rgba(0,0,0,0.7); */
  position: absolute;
  height: 300px;
  width: 290px;
  left: 0;
  top: 0;
  bottom: 0;
  right: 0;
  opacity: 0;
  -webkit-transition: all 0.4s ease-in-out 0s;
  -moz-transition: all 0.4s ease-in-out 0s;
  transition: all 0.4s ease-in-out 0s;
  /* border-radius: 10px; */
  margin-top: 10px;
 
}

.content:hover .content-overlay{
  opacity: 1;
}

.content-image{
  box-shadow:8px 8px 15px #e4e4e4;
  width: 100%;
  height: 300px;
  border-radius: 10px;
  margin-top:12px;
  object-fit: cover;
}

.content-details {
  position: absolute;
  text-align: center;
  padding-left: 1em;
  padding-right: 1em;
  width: 100%;
  top: 50%;
  left: 50%;
  opacity: 0;
  -webkit-transform: translate(-50%, -50%);
  -moz-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  -webkit-transition: all 0.3s ease-in-out 0s;
  -moz-transition: all 0.3s ease-in-out 0s;
  transition: all 0.3s ease-in-out 0s;
}

.content:hover .content-details{
  top: 50%;
  left: 50%;
  opacity: 1;
}
h5{
  color: #FF7779;
}

h6{
  color: #fff;
}
.content-details h3{
  color: #89CFF0;
  font-weight: 500;
  letter-spacing: 0.15em;
  margin-bottom: 0.5em;
  text-transform: uppercase;
}

.content-details p{
  color: #fff;
  font-size: 0.8em;
}

.fadeIn-bottom{
  top: 80%;
}

.fadeIn-top{
  top: 20%;
}

.fadeIn-left{
  left: 20%;
}

.fadeIn-right{
  left: 80%;
}


@media only screen and (max-width: 494px) {
    h1.headin{
    padding-top:50px;
}

.container {
  display: flex;
  justify-content: center;
  margin-right: auto;
  margin-left: auto;
}

.content{
  display: flex;
  justify-content: center;
  margin-right: auto;
  margin-left: auto;
}
}
</style>