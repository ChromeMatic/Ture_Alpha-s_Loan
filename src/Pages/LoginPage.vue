<template>
  <div class="loginBox">
  </div>
</template>

<script>
import NavBar from "@/components/NavBar";
export default {
  name: "LoginPage",
  components:{NavBar},
  data(){
    return{
      user:{
        username:"",
        password:""
      }
    }
  },
  computed:{},
  methods:{}
}
</script>

<style scoped>

</style>