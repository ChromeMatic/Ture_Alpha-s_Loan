<template>
<div>
    <NavBar/>
       <section>
         <div class="imgBox">
           <h1>Welcome</h1>
           <p>This is were your financial journey begins.</p>
         </div>
         <div class="contentBx">
             <div class="fromBx">
                <h1>Sign Up</h1>
               <form action="">

                <b-field label="Username">
                   <b-input
                       icon="account"
                       v-model="User.username"
                       placeholder="Please enter an username"
                   ></b-input>
                </b-field>

                 <b-field label="Email">
                   <b-input
                       icon="email"
                       type="email"
                       v-model="User.email"
                       placeholder="Please enter an email"
                   ></b-input>
                 </b-field>

                 <b-field label="Password">
                   <b-input
                       icon-pack="fas"
                       icon="key"
                       type="password"
                       v-model="User.password"
                   ></b-input>
                 </b-field>

                 <b-field label="Please enter password again.">
                   <b-input
                       icon-pack="fas"
                       icon="key"
                       type="password"
                       v-model="User.password_ch">
                   </b-input>
                 </b-field>

                 <div class="Bx">
                   <b-button class="btn" type="is-success" outlined>SIGN UP</b-button>
                 </div>
                 <div class="Bx">
                   <p>Have an account? <a href="/login">Sign in.</a></p>
                 </div>

               </form>
             </div>
         </div>
       </section>
    <Footer/>
</div>
</template>

<script>
import NavBar from "@/components/NavBar";
import Footer from "@/components/Footer";
export default {
  name: "SignUpPage",
  components:{NavBar,Footer},
  data(){
    return{
      User:{
        username:"",
        email:"",
        password:"",
        password_ch:""
      }
    }
  },
  computed:{
    check_(){},
    validation(){}
  },
  methods:{
    RegisterUser(){}
  }
}
</script>

<style scoped>
section{
  position: relative;
  width: 100%;
  height: 100vh;
  display: flex;
  color: #2c3e50;
  background:linear-gradient(-45deg,#fafafa,#ecf0f1);
}
section .imgBox{
  position: relative;
  width: 50%;
  height: 100%;
  background: linear-gradient(
      rgba(0,0,0,0.7),
      rgba(0,0,0,0.7) ) ,
  url('../assets/Img/SignUp-unsplash.jpg');
  background-size: cover;
  color: #FFFFFF;
  text-align: center;
}
.imgBox h1{
  margin-top: 13.5rem;
  font-weight: bold;
  font-size: 7.5rem;
}
.imgBox p{
   font-weight: 600;
   font-size: 2rem;
}

section .contentBx{
  display: flex;
  justify-content: center;
  align-items: center;
  width: 50%;
  height: 100%;
}
section .contentBx .fromBx{width: 50%;}

section .contentBx .fromBx h1{
  color:#2ecc71;
  font-weight: 600;
  font-size: 2.5rem;
  text-transform: uppercase;
  margin-bottom:1.4rem;
  display: inline-block;
  letter-spacing: 1px;
}

section .contentBx .fromBx .Bx{
  margin-bottom: 1rem;
  font-weight: 600;
}

@media only screen and (max-width: 768px){

  section .imgBox{
    position: absolute;
    top: 0;
    left:0;
    height: 100%;
    width: 100%;
  }
  .imgBox h1,p{display: none;}

  section .contentBx .fromBx h1{font-size: 2rem;}

  section .contentBx{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
    z-index: 1;
  }
  section .contentBx .fromBx{
    width: 100%;
    padding: 2rem;
    background: rgb(255 255 255 / 0.9);
    margin: 30px;
    border-radius:0.4rem ;
  }
  .btn{width: 100%;}
}
</style>