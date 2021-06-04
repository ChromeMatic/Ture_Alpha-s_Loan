<template>
 <nav class="menu">
   <ul class="nav-item">

     <li class="title">
       <h4>TrueAlphas</h4>
     </li>

      <li class="item">
        <a href="/Dashboard">Dashboard</a>
      </li>

     <li class="item">
       <a href="#">Account1</a>
     </li>

     <li class="item">
       <a href="#">Account2</a>
     </li>

     <li class="item">
       <a href="#">Account3</a>
     </li>

     <li class="Item">
       <a href="#">Settings</a>
     </li>

   </ul>
 </nav>
</template>

<script>
export default {
  name: "SideNav",
}
</script>

<style scoped>
 .menu{
   width: 5rem;
   height: 100Vh;
   position: fixed;
   background-color: #A1FFC6;
 }
 .nav-item{
   list-style: none;
   padding: 0;
   margin: 0;
   display: flex;
   flex-direction: column;
   align-items: center;
 }
 .item:last-child{
   margin-top: auto;
 }
</style>

