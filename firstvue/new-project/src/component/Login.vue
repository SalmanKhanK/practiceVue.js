<template>
<div>
<form>
  <Label>UserName</label>
  <input type="text" v-model="username">
  <Label>Password</label>
  <input type="password" v-model="Password">
  <button type="submit">Add</button>
  <div v-for="log in blog">
    <h3>{{log.UserName}}</h3>
  </div>
   
</form>
 
</div>

  
</template>

<script>

export default {

  data() {
    return {
     title:"Your first vue app",
     blog:[]
     
    }
  },
  created() {
          this.$http.get('backend/login.json').then(function(data) {
             console.log(data);
              this.blog=data.body
           })
          }
}
</script>

<style>


</style>
