<script >
export default {
  data() {
    return {
      images:["https://www.jquery-az.com/html/images/banana.jpg",'./src/assets/el.jpg',"./src/assets/klara.jpg","./src/assets/nikita.jpg"]
    }
  },
}
</script>

<template>

 <div class="container">
  <div v-for="img in images"><img v-bind:src=img></div>
 </div>
</template>

<style scoped>
.container{   padding: 10px;
  width: 100vw;
  min-height: 100vh;  background: #021927;
  display: flex;  flex-wrap: wrap; gap: 2rem;
  justify-content: space-evenly; align-items: center; overflow: hidden;
}
.container div{
  height: 350px;
  width: 200px;  
}
div img{
max-width: 300px;
width: 100%;
max-height: 600px; 
}
</style>
