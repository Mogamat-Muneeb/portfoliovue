<template>
 <div class="social1-menu">
        <ul>
            <li><a href="https://github.com/Mogamat-Muneeb" target="blank"><i class="fab fa-github"></i></a></li>
            <li><a href="https://www.linkedin.com/in/mogamat-muneeb-014769224/" target="blank"><i class="fab fa-linkedin-in"></i></a></li>

        </ul>
        <p class="p fw-bold ">© <span style="font-size:13.5px;">2022</span> Made with <i class="fa fa-heart"></i> by Mogamat Muneeb Davids</p>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.p{
    padding-top: 100px;
    color: #00bfff;
}
.social1-menu {
  position: relative;
  background:white;
    box-shadow:8px 8px 15px #e4e4e4;
  height:130px;
  width:100%;
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
    color: #012966;
    
}
.social1-menu ul li .fa{
    font-size: 30px;
    line-height: 50px;
    transition: .3s;
    color: #012966;
    
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
    background-color: #0077b5;
}


</style>