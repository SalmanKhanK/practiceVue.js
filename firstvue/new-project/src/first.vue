<template>
<div>
  <ul  v-for="fruiti in fruit">
     <li>
     {{fruiti}}
     </li>
  </ul>

</div>

  
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
       fruit:["Banana","Mango","Orange"]
    }
  }
}
</script>

<style>

</style>
