<template>
<div>
  <p>{{title}}</p>
 
  <app-header></app-header>
  <list></list>
  <first></first>
</div>

  
</template>

<script>
import header from './components/header.vue'
import first from './first.vue'
import list from './components/list.vue'
export default {
 components:{
   'app-header':header,
   'first':first,
   'list':list
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
