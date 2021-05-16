<template>
  <div class="panel1">

    <NavBar/>

    <div class="section sec1">
     <div class="title txt">
       <h1>Welcome To Ture Alpha's Loan</h1>
       <h3>Let us help you on your financial journey.</h3>
     </div>
    </div>

    <section class="section sec_box">
         <div class="box pd_Box">
          <div class="container">
            <h2 class="title has-text-centered is-size-3">
              How our service works
            </h2>

            <div class="columns mt-5 is-8 is-variable">

              <div class="column is-4-tablet is-3-desktop">

                <div class="card">
                  <div class="card-image has-text-centered px-6">
                    <img src="../Img/undraw_wallet_aym5.svg" alt="">
                  </div>
                  <div class="card-content">
                    <p class="title has-text-centered is-size-6">
                      Select the amount you want.
                    </p>
                  </div>
                </div>

              </div>

              <div class="column is-4-tablet is-3-desktop">

                <div class="card">
                  <div class="card-image has-text-centered px-6">
                    <img src="../Img/Form.svg" alt="">
                  </div>
                  <div class="card-content">
                    <p class="title has-text-centered is-size-6">
                      Complete our application form.
                    </p>
                  </div>
                </div>

              </div>

              <div class="column is-4-tablet is-3-desktop">

                <div class="card">
                  <div class="card-image has-text-centered px-6">
                    <img src="../Img/undraw_Reviewed_docs_re_9lmr.svg" alt="">
                  </div>
                  <div class="card-content">
                    <p class="title has-text-centered is-size-6">
                      Our financial experts will review your application.
                    </p>
                  </div>
                </div>

              </div>

              <div class="column is-4-tablet is-3-desktop">

                <div class="card">
                  <div class="card-image has-text-centered px-6">
                    <img src="../Img/approved.svg" alt="">
                  </div>
                  <div class="card-content">
                    <p class="title has-text-centered is-size-6">
                      Once approved, you collect your loan.
                    </p>
                  </div>
                </div>

              </div>

            </div>

          </div>
         </div>
    </section>

    <!-- Apply -->
    <section class="section sec2_box" id="apply">
      <div class="box">

        <div class="container" >
          <h2 class="title has-text-centered is-size-3">
            Apply today!
          </h2>

          <div class="columns is-desktop">

            <div class="column">

              <div class="card">
                <header class="card-header">
                  <p class="card-header-title">
                   How to Apply
                  </p>

                </header>
                <div class="card-content">
                    <div class="content">
                       To apply for a loan, you will have to complete
                       an application from. Once approved will will
                       be eligible to be granted the loan.
                    </div>
                  </div>
                <footer class="card-footer">
                    <a href="#" class="card-footer-item btn">APPLY NOW</a>
                </footer>
              </div>

            </div>

          </div>

        </div>

      </div>
    </section>

    <!-- About Us -->
    <section id="About_Us" class="section sec3_box">

      <div class="box">
        <div class="container">

          <h2 class="title has-text-centered is-size-3">
            About Us
          </h2>
          <div class="columns is-desktop">

            <div class="column">
              <div class="card">
                <header class="card-header">
                  <p class="card-header-title">
                    True Alpha's Loan
                  </p>

                </header>
                <div class="card-content">
                  <div class="content" >
                    <p>
                      True Alpha’s is a small financial institution that grants small loans to individuals
                      that meets the requirements. True Alpha’s was founded by [insert name of person]
                      who is know the ceo of the company on the date of [insert date].
                    </p>
                  </div>
                </div>
                <footer class="card-footer">
                  <a href="#" class="card-footer-item btn">Learn more</a>
                </footer>
              </div>
            </div>

          </div>
        </div>
      </div>

    </section>

    <!-- Contact Us -->
    <section class="section sec3_box" id="Contact">

       <div class="box">
         <div class="container">
           <h2  class="title has-text-centered is-size-3">
             Contact Us
           </h2>
           <div class="columns is-desktop">

             <div class="column">
               <div class="card">
                 <header class="card-header">
                   <p class="card-header-title">
                     Contact Information
                   </p>

                 </header>
                 <div class="card-content">
                   <div class="content">
                      <p>Number: 1(860)775-5231</p>
                      <p>Email : TrueAlphaLoan@gmail.com</p>
                   </div>
                 </div>
               </div>
             </div>

           </div>
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
  name: "LandingPage",
  components:{
    NavBar,
    Footer
  }
}
</script>

<style >
  .panel1{
    margin: 0;
    padding: 0;
  }
 .sec1{
   display: flex;
   justify-content: center;
   align-items: center;
   height: 36em;
   background: linear-gradient(
       rgba(0,0,0,0.7),
       rgba(0,0,0,0.7) ) ,
   url('../Img/rupixen-com-o9YWMdUoW8I-unsplash.jpg');
   background-size: cover;
 }
 .title h1{
   color: #FFFFFFFF;
   font-size: 6.5rem;
 }

 .txt{text-align: center;}
 .txt h3{color: #FFFFFFFF;}
 .sec_box{background-color: #A1FFC6;}
 .sec2_box{background-color: #A1FFC6;}
 .sec3_box{background-color: #A1FFC6}
 .cont_ h1{margin-top: 7rem;}

 .btn{
   font-weight: bolder;
 }
 .btn:hover{
   transition: ease-in 0.3s;
   color:#2ecc71;
 }
  @media only screen and (max-width: 1024px){
    .pd_Box{padding: 1rem 0;}
  }
  @media only screen and (max-width: 600px) {
    .title h1{font-size: 3rem;}
    .txt h3{
      margin-top: 1rem;
      font-size: 1.2rem;
    }
    .cont_ h1{margin-top: 2rem;}
  }
</style>

