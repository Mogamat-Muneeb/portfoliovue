<template>
  <h1 class="headin d-flex justify-content-center"><span  style="color:#1e90ff;">Skills</span> </h1>
  <div class="container  d-flex justify-content-center">
    <div class="row">
      <div class="col">
         <div class="logo">
           <img src="../assets/html5.png">  
             <span class="logotext">HTML5</span>
        </div>
        
         <div class="logo">
            <img src="../assets/css.png">
              <span class="logotext">CSS</span>
        </div>
        <div class="logo">
            <img src="../assets/bootstrap.png">
            <span class="logotext">BOOTSTRAP</span>
        </div>
         <div class="logo">
           <img src="../assets/javascript.png">  
              <span class="logotext">JAVASCRIPT</span>
        </div>
        <div class="col">
            <div class="logo">
           <img src="../assets/vue.png">  
              <span class="logotext">VUE</span>
        </div>
           <div class="logo">
           <img src="../assets/node.png">  
              <span class="logotext">NODE</span>
        </div>
           <div class="logo">
           <img src="../assets/mysql.png">  
              <span class="logotext">MYSQL</span>
        </div>
        </div>
       
         </div>
         <h1 class="head d-flex justify-content-center"><span  style="color:#1e90ff;">Tools</span> </h1>
         <div class="col">
          <div class="logo">
            <img src="../assets/vscode.png">  
               <span class="logotext">VSCODE</span>
        </div>
        
          <div class="logo">
            <img src="../assets/git.png">  
            <span class="logotext">GIT</span>
        </div>
          <div class="logo">
            <img src="../assets/cmd.png"> 
            <span class="logotext">CMD</span>
        </div>
          <div class="logo">
            <img src="../assets/npm.png">  
            <span class="logotext">NPM</span>
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


/* logo text */
.logo .logotext {
  visibility: hidden;
  width: 120px;
  background-color:#00bfff;
  color: #fff;
  text-align: center;
  padding: 5px 0;
  border-radius: 6px;
  position: absolute;
  z-index: 1;
  
}


.logo:hover .logotext {
  visibility: visible;
}
h1.headin{
    padding-top:110px;
}

.head{
  margin-top:30px;
}
.col{
  margin-top:30px;
}
.logo{
    position: relative;
  display: inline-block;
  display:inline-flex;
  justify-content: center;
  flex-wrap: wrap;
  margin: 5px;
  border-radius:10px;
  border:5px solid white;
  box-shadow:8px 8px 15px #e4e4e4;
  margin-bottom:50px;
}
.logo:hover{
  transform: translate(-3px, -3px);
}
img{
  width:125px;
  height:125px;
  object-fit: cover;
  margin: 10px;
}

@media only screen and (max-width: 494px) {
    h1.headin{
    padding-top:50px;
}
}

</style>