<template>
  <div class="bg">
    <SideNav/>
    <section class="section info">
      <h1>Title</h1>
      <p>
        Lorem ipsum dolor sit amet, consectetur
        adipisicing elit. Accusamus accusantium
        ad amet aspernatur autem consequuntur
        cum cupiditate deleniti distinctio
        doloremque earum exercitationem
        explicabo facere fuga, fugiat itaque
        laudantium libero minus,
      </p>

      <h1>Title</h1>
      <p>
        Lorem ipsum dolor sit amet, consectetur
        adipisicing elit. Accusamus accusantium
        ad amet aspernatur autem consequuntur
        cum cupiditate deleniti distinctio
        doloremque earum exercitationem
        explicabo facere fuga, fugiat itaque
        laudantium libero minus,
      </p>

      <h1>Title</h1>
      <p>
        Lorem ipsum dolor sit amet, consectetur
        adipisicing elit. Accusamus accusantium
        ad amet aspernatur autem consequuntur
        cum cupiditate deleniti distinctio
        doloremque earum exercitationem
        explicabo facere fuga, fugiat itaque
        laudantium libero minus,
      </p>

      </section>
  </div>
</template>

<script>
import SideNav from "@/components/SideNav";
export default {
  name: "Dashboard",
  components:{SideNav}
}
</script>

<style scoped>
.bg{
  display: flex;
  flex-direction: row;
}
.info{
  margin-left: 5rem;
  padding: 1rem;
}
</style>