<template>


<h1 class="headin d-flex justify-content-center fw-bold"><span  style="color:#1e90ff;">Contact Me</span> </h1>
  <div class="containe d-flex justify-content-center" id="contact">


    <div class="row">

        <div class="  ">
                <div class="call  row "> 
                <div class="call-holder col-md-4 col-lg-4"  > <i class="fas fa-phone-alt " ></i> 
                  <br> 
                      <div class="call-me fw-bold ">Call Me On:</div>
                      <div class="call-me-1 text-muted">+ 27 76 162 1649</div>
                </div>

                <div class="call-holder  col-md-4 col-lg-4"> <i class="fas fa-map-marker-alt"  ></i> 
                  <br> 
                      <div class="call-me fw-bold">Home:</div>
                      <div class="call-me-1 text-muted">Cape Town, South Africa</div>
                </div>

                <div class="call-holder  col-md-4 col-lg-4"> <i class="fas fa-envelope" ></i> 
                  <br> 
                      <div class="call-me fw-bold">Email:</div>
                      <div class="call-me-1 text-muted">davimuneeb785@gmail.com</div>
                </div>
            </div>
       
            <form @submit.prevent="handleSubmit" id="contact-form" name="myForm" class="form"  role="form">

                <div class="form-group">
                    <label class="form-label" id="nameLabel" for="name"></label>
                    <input type="text" class="form-control" id="name" name="name" placeholder="e.g. John Doe" tabindex="1"  required v-model="name">
                    
                </div>

                <div class="form-group">
                    <label class="form-label" id="emailLabel" for="email"></label>
                    <input type="email" class="form-control" id="email" name="email"   placeholder="e.g. john.doe@gmail.com" tabindex="2" required v-model="email">
                </div>

                <div class="form-group">
                    <label class="form-label" id="subjectLabel" for="sublect"></label>
                    <input type="text"  class="form-control" id="subject" name="subject" placeholder="Phone number" tabindex="3" required v-model="contact">
                </div>

                <div class="form-group">
                    <label class="form-label" id="messageLabel" for="message"></label>
                    <textarea rows="6" cols="60" name="message" class="form-control" id="message" placeholder="Write message..." tabindex="4" v-model="message"></textarea >                                 
                </div>

                <div class=" b text-center margin-top-25">
                    <button type="submit" class="btn btn-mod btn-border btn-large"> <span class="log" v-show="!loading">Send Message</span>
                      <span v-show="loading"><Loader/></span></button>
                    <button type="reset" value="Reset" class="btn btn-mod btn-border btn-large">reset</button>
                </div>

            </form>
          
        </div>

    </div>
    
  </div>
</template>

<script>
import Loader from "../components/Loader.vue"
export default {
  data(){
    return {
      name:"",
      email: "",
      contact: "",
      message: "",
      loading: "",

    }
  },
          components:{ Loader },

  methods:{
    handleSubmit(){
    this.loading = true;
    console.log(this.name,this.email,this.contact,this.message)
    fetch('https://myport-backend.herokuapp.com/contact', {
  method: 'POST',
  body: JSON.stringify({
    name: this.name,
    email: this.email,
    contact: this.contact,
    message: this.message,
  }),
  headers: {
    'Content-type': 'application/json; charset=UTF-8',
  },
})
  .then((response) => response.json())
  .then((json) =>{alert(json.msg);
  this.loading=false} )
  .catch((error) => alert(error.msg));
    }
  }
}
</script>

<style scoped>
 
textarea#message.form-control {
    height: 120px;
}
h1.headin{
    padding-top:110px;
}
:required:hover{
  background-color:none;
}

*{
  scroll-behavior: smooth;
}
.containe {
  display:flex;
  padding: none;

  /* height:100vh; */
  margin-bottom: 20px;
}
/* contact */
#success-message {
  opacity: 0;
}

.col-xs-12.col-sm-12.col-md-12.col-lg-12 {
  padding: 0 20% 0 20%;
}

.margin-top-25 {
  margin-top: 25px;
}

.form-title {
  padding: 25px;
  font-size: 30px;
  font-weight: 300;

}

.form-group .form-control {
   display: block;
    border-radius: 0;
    width: 100%;
    height: 48px;
    padding: 10px 24px;
    font-size: 15px;
    font-weight: 400;
    border-radius: 25px;
    line-height: 1.6;
    color: #333;
    background-color: #fff;
    background-image: none;
    border: solid 1px #9dd8e0;
    -webkit-box-shadow: none;
  
     box-shadow:8px 8px 15px #e4e4e4;
}


.form-group .form-control:hover {
	border: solid 1px#1e90ff;
}



.btn-mod.btn-large {
    height: auto;
    padding: 13px 52px;
    font-size: 15px;
    
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
    text-decoration: none;
    letter-spacing: 2px;
    -webkit-border-radius: 0;
    -moz-border-radius: 0;
    border-radius: 0;
    -webkit-box-shadow: none;
    -moz-box-shadow: none;
    box-shadow: none;
    -webkit-transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
    -moz-transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
    -o-transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
    -ms-transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
    transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
}

.btn-mod.btn-border:hover, .btn-mod.btn-border:active, .btn-mod.btn-border:focus, .btn-mod.btn-border:active:focus {
     color:  #012966;
    border-color:#9dd8e0 ;
    background:#9dd8e0;
    outline: none;
    
}

@media only screen and (max-width: 500px) {
    .btn-mod.btn-large {
       padding: 11px 15px;
       font-size: 14px;
    }
  
    .form-title {
        font-size: 20px;
  }
  .containe{
    padding: 80px;
  }
}


.fas{
  display:flex;
  justify-content: center;
  font-size:35px;


  
}

.call-me{
  display:flex;
  justify-content: center;
  color:#9dd8e0;
}

.call-me-1{
  display:flex;
  justify-content: center;

}
.call-holder{
  padding-top: 15px;
}
.fas{
  color:#1e90ff;
}
.b{
  display:flex;
  justify-content: space-around;
  
  
}

.btn{
    
    padding: 25px 43px;
    border-radius: 30px;

    


}




@media only screen and (max-width: 494px) {
    h1.headin{
    padding-top:50px;
}
}
</style>