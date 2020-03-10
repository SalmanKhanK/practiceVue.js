<template>
<div>
  <p>{{title}}</p>
  <Login></Login>
</div>

  
</template>

<script>
  import Login from './component/Login.vue'
export default {

 components:{
     'Login' :Login
 },
  data() {
    return {
     title:"Your first vue app"
    }
  }
}
</script>

<style scoped>
p{
  color:green;
}

</style>
