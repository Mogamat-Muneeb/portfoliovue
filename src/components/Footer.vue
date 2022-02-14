<template>
<!-- <footer class="footer"> -->
 
 <div class="social1-menu">
        <ul>
            <li><a href="https://github.com/Mogamat-Muneeb" target="blank"><i class="fab fa-github"></i></a></li>
            <!-- <li><a href="https://www.instagram.com/muneeb_davids/" target="blank"><i class="fab fa-instagram"></i></a></li> -->
            <li><a href="https://www.linkedin.com/in/mogamat-muneeb-014769224/" target="blank"><i class="fab fa-linkedin-in"></i></a></li>
            <li><a href="https://codepen.io/your-work" target="blank"><i class="fab fa-codepen" target="blank"></i></a></li>
            <!-- <li><a href="https://app.netlify.com/teams/mogamat-muneeb/overview" target="blank"><i class="fa fa-link" target="blank"></i></a></li> -->

        </ul>
        <p class="p fw-bold ">© <span style="font-size:13.5px;">2022</span> Made with <i class="fa fa-heart" aria-hidden="true"></i> by Mogamat Muneeb Davids</p>
  </div>
<!-- </footer> -->
 

</template>

<script>
export default {

}
</script>

<style scoped>



.p{
    padding-top: 100px;
    color: #89CFF0;
}
.social1-menu {
  position: relative;
  background: #f5f5f5;
    box-shadow:8px 8px 15px #ababab;
  height:130px;
}


.social1-menu ul{
    position: absolute;
    top: 50%;
    left: 50%;
    padding: 0;
    margin: 0;
    transform: translate(-50%, -50%);
    display: flex;
    padding-bottom:30px;
    

}

.social1-menu ul li{
    list-style: none;
    margin: 0 15px;
}

.social1-menu ul li .fab{
    font-size: 30px;
    line-height: 50px;
    transition: .3s;
    color: #000;
    
}
.social1-menu ul li .fa{
    font-size: 30px;
    line-height: 50px;
    transition: .3s;
    color: #000;
    
}

.social1-menu ul li .fab:hover{
    color: #fff;
}
.social1-menu ul li .fa:hover{
    color: #fff;
}

.social1-menu ul li a{
    position: relative;
    display: block;
    width: 47px;
    height: 47px;
    border-radius: 50%;
    background-color: #fff;
    text-align: center;
    transition: .6s;
    box-shadow: 0 5px 4px rgba(0,0,0,.5);
}

.social1-menu ul li a:hover{
    transform: translate(0, -10%);
}

.social1-menu ul li:nth-child(1) a:hover{
    background-color: rgba(0, 0, 0, 0.829);
}
.social1-menu ul li:nth-child(2) a:hover{
    background-color: #E4405F;
}
.social1-menu ul li:nth-child(3) a:hover{
    background-color: #0077b5;
}
/* .social1-menu ul li:nth-child(4) a:hover{
    background-color: #000;
}
.social1-menu ul li:nth-child(5) a:hover{
    background-color: rgb(0, 187, 255);
} */

</style>