<template>
<nav id="nav" class="links" :class="{ active: isActive}">
  
    <router-link @click="toggleNav" to="/">Home</router-link>
     <router-link @click="toggleNav" :to="{ name: 'About'}">About</router-link>
    <router-link @click="toggleNav" :to="{ name: 'Resume'}">Resume</router-link>
    <router-link @click="toggleNav" :to="{ name: 'Skills'}">Skills</router-link>
    <router-link @click="toggleNav" :to="{ name: 'Projects'}">Projects</router-link>
    <router-link @click="toggleNav" :to="{ name: 'Testimonials'}">Testimonials</router-link>
    <router-link @click="toggleNav" :to="{ name: 'Contact'}">Contact</router-link>
</nav>    
<button id="nav-btn" @click="toggleNav">
    <i class="fa fa-bars"></i>
</button>    

</template>

<script>
export default {
    data(){
        return {
            isActive: false,
        };
    },
    methods:{
        toggleNav() {
            this.isActive = !this.isActive;
        },
    },
};
</script>

<style scoped>

.links{
    
    display:flex;
    justify-content:end;
    gap: 10px;      
}
#nav{
    
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 75px;
    background: #f5f5f5;
    box-shadow:8px 8px 15px #e4e4e4;

    
}

#nav-btn{
    position: fixed;
    top: 10px;
    right: 10px;
    background: #f5f5f5;
    box-shadow:8px 8px 15px #e4e4e4;
    padding: 10px;
    border-radius: 50%;
    border: none;
    outline: none;
    display: none;
    overflow: hidden;
}
 /* #nav{
    padding: 10px;


a {
    font-weight:bold;
    color: #2c3e50;
    padding: 10px;
    text-decoration: none;
    &.router-link-exact-active{
        color: #42b983;
    }
}
}  */

@media screen and (max-width:500px) {
    #nav{
        height:100%;
        left: -100vw;
        display:flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        transition:left 0.1s linear;
            gap: 40px;
    }
    #nav.active{
        left:0;
    }
    #nav-btn{
        display:block;

        
    }
}
</style>