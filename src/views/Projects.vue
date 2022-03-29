<template>
 <h1 class="headin d-flex justify-content-center"><span  style="color:#1e90ff;">Projects</span> </h1>
   <span v-show="loading"><Loader/></span>


  <div class="container">
     <div v-for="project in projects" :key="project.id" class="project">
        <div class="proj_box">
            <!-- <h2>{{ project.title }}</h2> -->
            <div class="bucket">
            <img class="proj_img" :src="project.img" alt="">
            <div class="overlay">
            <div class="text1 fw-bolder">{{ project.title }}</div>
            
                <div class="econ">
                <div class="row">
                  <p>{{ project.desc }}</p>
                <div class="col">
                <a :href="project.github" target="_blank"><i class="   fab fa-github"></i></a> 
                 </div>
                <div class="col">
                 <a :href="project.netlify" target="_blank"><i class=" far fa-eye"></i></a> 

                 </div>
                </div>
            </div>
            </div>
         </div>
        </div>
     </div>
  </div>
 
</template>

<script>
import Loader from "../components/Loader.vue"
export default {
        data(){
            return {
                projects:[],
                loading: false
            }
        },
        components:{ Loader },
        mounted(){
          this.loading = true
            fetch("https://myport-backend.herokuapp.com/projects")
            .then(res => res.json())
            .then(data => {this.projects = data;
            this.loading =  false} )
            .catch(err => console.log(err.message))
            
            
        }
       
}


</script>

<style scoped>
h1.headin{
    padding-top:80px;
}
p{
  position:relative;
  bottom: 55px;
  color: white;
  
}
.container {
    display:flex;
    justify-content: center;
    flex-wrap: wrap;
    overflow-y: hidden;
    margin-top:15px ;
    position: initial;
    margin-bottom:50px;
    /* height:70vh; */
      height:100vh;
}
.project{
    display: flex;
    justify-content:center;
    flex-wrap: wrap;
    position:initial;
}

.bucket {
    display:flex;
    justify-content: center;
    flex-wrap: wrap;
    width: 400px;
    height: 250px;
    position: relative;
    margin: 10px;
  
}

.proj_img {
  display: block;
  width: 399px;
  height: auto;
  object-fit: cover;
   /* border: 6px solid lightgray; */
   
  border: 6px solid white;
  border-radius:6px;
  box-shadow:8px 8px 15px #e4e4e4;
  
}

.overlay {
   
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: .5s ease;
  background: rgba(0, 0, 0, 0.5);
  border-radius:6px;
}

.bucket:hover .overlay {
  opacity: 1;
  
  
  
}


.text1 {
  color: #00bfff;
  font-size: 20px;
  position: absolute;
  top: 30%;
  left: 30%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);

  text-align: center;
 

  
}
.fab:hover{
    color:#1e90ff;
     
}
.far:hover{
    color:#1e90ff;
     
}

.fab{
    font-size:30px;
    display: column;
    color: white;
    float: left;
    padding-left: 260px;
}
.far{
    font-size:30px;
    display: column;
    color: white;
    /* padding-left: 40px; */
}

.econ{
    display:flex;
    justify-content: space-evenly;
    padding-top: 145px;
}


@media only screen and (max-width: 904px){
  .bucket {
  display:flex;
  justify-content: center;
  flex-wrap: wrap;
  width: 350px;
  height: 250px;
  position: relative;
  margin: 10px;
 
}

.proj_img {
  display: block;
  width: 350px;
  height: auto;
  object-fit: cover;
  border: 6px solid white;
  border-radius:6px;
  
}
p{
  position:relative;
  bottom: 40px;
  color: white;
  
}

.overlay {
   
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: .5s ease;
  background: rgba(0, 0, 0, 0.5);
  border-radius:6px;
}

.text1 {
  color: #00bfff;
  font-size: 20px;
  position: absolute;
  /* top: 50%; */
  left: 50%;
  /* padding-right: 10px; */
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);

  text-align: center;
 

  
}
.fab{
  padding-top: 25px;
    font-size:30px;
    display: column;
    color: white;
    float: left;
    padding-left: 15px;
      padding-right: 15px;
}
.far{
    padding-top: 25px;
    font-size:30px;
    display: column;
    color: white;
    /* padding-left: 40px; */
}

}

h1{
  margin-top:40px;
}


@media only screen and (max-width: 494px) {
    h1.headin{
    padding-top:3px;
}
.fab{
  padding-top:-1px;
    font-size:25px;
    /* display: column; */
    color: white;
    /* float: left; */
    /* padding-left: 15px; */
      /* padding-right: 15px; */
}
.far{
    padding-top:-1px;
    font-size:25px;
    /* display: column; */
    color: white;
    /* padding-left: 40px; */
}
.econ{
    /* display:flex; */
    /* justify-content: space-around; */
    padding-top: 145px;
}
p{
  position:relative;
  bottom: 40px;
  color: white;
  
}

.col{
  padding-left:70px;
  padding-right:70px;
  position: relative;
  bottom: 50px;
}
}
</style>