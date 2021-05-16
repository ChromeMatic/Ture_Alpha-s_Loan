<template>
  <b-navbar class="is-link" :fixed-top="true"  :transparent="true" >

    <template #brand>
      <b-navbar-item tag="router-link" :to="{ path: '/' }">
        <img src="../Img/TURE ALPHA.png">
      </b-navbar-item>
    </template>

    <template #start>
      <b-navbar-item href="/">
        Home
      </b-navbar-item>

      <b-navbar-item href="#About_Us">
        About Us
      </b-navbar-item>

      <b-navbar-dropdown label="Services">
        <b-navbar-item href="#apply">
          Apply for loan
        </b-navbar-item>
        <b-navbar-item href="#Contact">
          Contact Us
        </b-navbar-item>
      </b-navbar-dropdown>

    </template>

    <template #end>
      <b-navbar-item tag="div">
        <div class="buttons">
          <a class="button is-primary" href="/signUp">
            <strong>Sign up</strong>
          </a>
          <a class="button is-light" href="/login">
            Log in
          </a>
        </div>
      </b-navbar-item>
    </template>

  </b-navbar>
</template>

<script>
export default {
  name: "NavBar",
  created() {
    window.addEventListener('scroll', this.handleScroll);
  },
  destroyed () {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods:{
    handleScroll (event) {
      let scrollpos = window.scrollY
      const header = document.querySelector("nav")
      const header_height = header.offsetHeight

      const add_class_on_scroll = () => header.classList.add("isActive")
      const remove_class_on_scroll = () => header.classList.remove("isActive")

      window.addEventListener('scroll', function() {
        scrollpos = window.scrollY;

        if (scrollpos >= header_height) {
          add_class_on_scroll();
          console.log(add_class_on_scroll);
        }
        else {
          remove_class_on_scroll();
          console.log(remove_class_on_scroll);
        }

      })
    }
  }
}
</script>

<style>
nav.navbar.is-fixed-top {
  transition: background-color 0.5s ease;
  background: transparent;
}

nav.navbar.is-fixed-top.isActive{
  transition: background-color 0.5s ease;
  background:black;
}

/* add top overlay for more readable navbar text */
#overlay{
  background: linear-gradient(to top, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.55));
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  z-index: 1;
}

img.responsive_img{
  width: 100%;
  height: auto;
}
body{padding-top: 0px!important;}
</style>
