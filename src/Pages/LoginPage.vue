<template>
  <div>
    <NavBar/>
    <section>
      <div class="imgBx">
         <h1>Welcome Back</h1>
      </div>

      <div class="contentBx">
        <div class="formBx">
          <h1>Login</h1>

          <form action="">

            <b-field class="inputBx" label="Email">
              <b-input icon="email" type="email" v-model="user.email"></b-input>
            </b-field>

            <b-field class="inputBx" label="Password">
              <b-input type="password" v-model="user.password"></b-input>
            </b-field>

            <b-field class="inputBx">
              <b-checkbox class="remember" v-model="user.checkbox"> Remember Me</b-checkbox>
            </b-field>

            <div class="inputBx">
              <b-button class="btn" type="is-success" outlined>LOGIN</b-button>
            </div>

            <div class="inputBx">
              <p>Don't have an account? <a href="/signUp">Sign up.</a></p>
            </div>
          </form>

          <h2>Login with social media</h2>
          <ul class="social_links">
            <li><a href="#"><i class="fab fa-google"></i></a></li>
            <li><a href="#"><i class="fab fa-facebook-square"></i></a></li>
            <li><a href="#"><i class="fab fa-twitter"></i></a></li>
            <li><a href="#"><i class="fab fa-linkedin"></i></a></li>
          </ul>

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
  name: "LoginPage",
  components:{NavBar,Footer},
  data(){
    return{
      user:{
        email:"",
        password:"",
        checkbox:false
      }
    }
  },
  computed:{},
  methods:{}
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
 section .imgBx{
   position: relative;
   width: 50%;
   height: 100%;
   background: linear-gradient(
       rgba(0,0,0,0.6),
       rgba(0,0,0,0.6) ) ,
   url('../assets/Img/Login-unsplash.jpg');
   background-size: cover;
 }
 .imgBx h1{
   margin-top: 13.5rem;
   font-weight: bold;
   font-size: 6.5rem;
   color: #FFFFFF;
   text-align: center;
 }
 section .contentBx{
   display: flex;
   justify-content: center;
   align-items: center;
   width: 50%;
   height: 100%;
 }
 section .contentBx .formBx{width: 50%;}
 section .contentBx .formBx h1{
   color:#2ecc71;
   font-weight: 600;
   font-size: 2.5rem;
   text-transform: uppercase;
   margin-bottom:1.4rem;
   display: inline-block;
   letter-spacing: 1px;
 }

 section .contentBx .formBx .inputBx{
   margin-bottom: 1rem;
 }

 .remember{font-weight: 600;}
 .inputBx{font-weight: 600;}
 section .contentBx .formBx h2{
   font-weight: 600;
   text-align: center;
   margin: 50px 0 8px;
 }
 section .contentBx .formBx .social_links{
   display: flex;
   justify-content: center;
   align-items: center;
 }
 section .contentBx .formBx .social_links li a{
   list-style: none;
   text-decoration: none;
   width: 3.125rem;
   height: 3.125rem;
   display: flex;
   justify-content: center;
   align-items: center;
   cursor: pointer;
   color:#2c3e50;
 }
 section .contentBx .formBx .social_links li a{
   font-size: 1rem;
   transition: color 0.4s ease;
 }
 section .contentBx .formBx .social_links li a:hover{
   color: #2ecc71;
 }

 @media only screen and (max-width: 768px){
     section .imgBx{
       position: absolute;
       top: 0;
       left:0;
       height: 100%;
       width: 100%;
     }

   .imgBx h1{
     display: none;
   }

   section .contentBx .formBx h1{
     color:#2ecc71;
     font-weight: 600;
     font-size: 2rem;
     text-transform: uppercase;
     margin-bottom:1.4rem;
     display: inline-block;
     letter-spacing: 1px;
   }

     section .contentBx{
       display: flex;
       justify-content: center;
       align-items: center;
       width: 100%;
       height: 100%;
       z-index: 1;
     }
     section .contentBx .formBx{
       width: 100%;
       padding: 2rem;
       background: rgb(255 255 255 / 0.9);
       margin: 30px;
       border-radius:0.4rem ;
     }
   section .contentBx .formBx h2{
     font-weight: 600;
     text-align: center;
     margin: 30px 0 8px;
   }

   .btn{
     width: 100%;
   }
 }


</style>