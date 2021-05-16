<template>
    <div class="_footer">
      <footer class="f_p">

          <div class="f_content">
            <h2>Social Media Links</h2>
            <p> Follow us online!</p>
             <ul class="social_Links">
               <li><a href="#"><i class="fab fa-facebook-square"></i></a></li>
               <li><a href="#"><i class="fab fa-instagram"></i></a></li>
               <li><a href="#"><i class="fab fa-twitter"></i></a></li>
             </ul>
          </div>
      </footer>
      <div class="footer-bottom">
        <p>Copyright &copy 2021 True Alpha's Loan.</p>
      </div>
    </div>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style scoped>
   ._footer{
     background-color: #111;
     margin: 0;
     padding: 0;
     display: flex;
     flex-direction: column;
     text-align: center;
     align-items: center;
     justify-content: center;
   }
   .f_p{
     padding: 0.2rem 0;
   }
   .f_p p{
     margin: 0.8rem 0;
     color: #FFFFFFFF;
     font-weight: bold;
     line-height: 1rem;
   }
   .f_content h2{
     margin-top: 0.4rem;
     font-size: 1.6rem;
     font-weight: bold;
     color: #FFFFFF;
   }
   .social_Links{
     list-style: none;
     display: flex;
     justify-content: center;
     align-items: center;
     margin: 1.2rem 0.5rem;
   }
   .social_Links li{margin: 0 0.6rem;}
   .social_Links a{
     text-decoration: none;
     color: #FFFFFF;
   }
   .social_Links a i{
     font-size: 1.4rem;
     transition: color 0.4s ease;
   }

   .social_Links a:hover i{
     color: #2ecc71;
   }

   .footer-bottom{
     background-color: black;
     width: 100vw;
     padding: 0.7rem 0;
   }

   .footer-bottom p{
     font-weight: bold;
     color: #FFFFFF;
   }

</style>