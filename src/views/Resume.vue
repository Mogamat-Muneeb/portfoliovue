<template>
 <h1 class="headin d-flex justify-content-center"><span  style="color:#1e90ff;">Resume</span> </h1>
       
      <h3  style="color:#00bfff;">Education</h3>
      <div class="card">
      <div class="info">
        <h4 class="date" style="font-size:13px;font-weight:bold; "><i class="fas fa-graduation-cap"></i> 2016-2020:</h4>
        <h3 class="title" style="font-weight:bold;color:#1e90ff;">Vootrekker High School</h3>
        <p style="font-weight:500">I started and matriculated at Voortrekker High School in Kenilworth. I was part of the RCL leadership team from Gr.10 to Gr.12 and played First-Team rugby since Gr.10 as a Scrumhalf. As well as being the Deputy Head Boy in Matric. </p>
    </div>
      </div>
      <div class="card">
        <div class="info">
        <h4 class="date" style="font-size:13px;font-weight:bold; "><i class="fas fa-graduation-cap"></i> 2021-Present:</h4>
        <h3 class="title" style="font-weight:bold;color:#1e90ff;">Life Choices Coding Academy</h3>
        <p style="font-weight:500">A Bootcamp program that provides you with the core fundamentals of Web Development, learning coding languages such as HTML, CSS, JavaScript, and more coding techniques. We taught interpersonal and self-development skills to take us further in life. </p>
    </div>
      </div>
    <h3  style="color:#00bfff;">Work & Experience</h3>
      <div class="card">
        <div class="info">
        <h4 class="date" style="font-size:13px;font-weight:bold; "><i class="fas fa-briefcase"></i> 2014-2018:</h4>
        <h3 class="title" style="font-weight:bold;color:#1e90ff;">Project Maritime Youth</h3>
        <p style="font-weight:500">Every Saturday for four years, I spent my day practicing naval and survival skills. I was also an instructor and PTI officer. I improved my leadership and discipline due to harsh and intense physical training.</p>
    </div>
      </div>
        <div class="card">
        <div class="info">
        <h4 class="date" style="font-size:13px;font-weight:bold; "><i class="fas fa-briefcase"></i> Start of 2021:</h4>
        <h3 class="title" style="font-weight:bold;color:#1e90ff;">Kieth Sealants and Projects</h3>
        <p style="font-weight:500"> I was an apprentice, learning general building techniques.</p>
    </div>
      </div>
       <div class="card">
        <div class="info">
        <h4 class="date" style="font-size:13px;font-weight:bold; "><i class="fas fa-briefcase"></i> 2020-present:</h4>
        <h3 class="title" style="font-weight:bold;color:#1e90ff;">Volunteering</h3>
        <p style="font-weight:500"> Started tutoring and helping out at Muslim school, teaching kids how to recite the Quran and fundamentals of Islam and tutoring mathematics to grade 9 learners.</p>
    </div>
      </div>
       <div class="card">
        <div class="info">
        <h4 class="date" style="font-size:13px;font-weight:bold; "><i class="fas fa-briefcase"></i> Feb 2022-present:</h4>
        <h3 class="title" style="font-weight:bold;color:#1e90ff;">Lc Studio</h3>
        <p style="font-weight:500">An internship where the fundamentals of working in actual web apps teams is put into practice. As well as upskilling myself in coding. </p>
       </div>
      </div> 

     
      
  
</template>

<script>
export default {

}
</script>

<style scoped>
.fas{
 color: #00bfff;
 font-size:17px;

}
h1.headin{
    padding-top:110px;
}
h1{
  padding-top:50px;
}
.card{
    text-align:left;
    background: none;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    margin-right:auto;
    margin-left:auto;
    position: initial;
    width:70%;
    height:270px;
    border-radius:10px;
    margin-top:20px;
    border:5px solid white;
      box-shadow:8px 8px 15px #e4e4e4;
    margin-bottom:50px;
}

.card:hover{
  transform: scale(1.1);
  transition:.5s;
}

.info {
    
    padding-left: 20px;
}


@media only screen and (max-width: 494px) {
    h1.headin{
    padding-top:50px;
}

h3{
  font-size:18px;
}
}
</style>