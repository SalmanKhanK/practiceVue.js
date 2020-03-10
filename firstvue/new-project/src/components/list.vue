<template>
<div id="list">
   <ul>
     <li v-for="lists in list" v-on:click="lists.show=!lists.show">
     <h2>
        {{lists.name}}
     </h2>
     <h3 v-show="lists.show">
     {{lists.sirName}}
     </h3>
     
     </li>
   </ul>
</div> 
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      list:[
          {name:'Roy','sirName':'Dunk',show:false},
          {name:'lee','sirName':'white',show:false},
          {name:'fari','sirName':'jasson',show:false},
          {name:'hui','sirName':'jack',show:false},
      ]
    }
  }
}
</script>

<style scoped>
#list{
    width:100%;
    max-width:1200px;
    margin:40px auto;
    padding: 0 20px;
    box-sizing:border-box;

}
ul{
    display: flex;
    flex-wrap: wrap;
    list-style-type: none;
    padding: 0;
}
li{
    flex-grow: 1;
    flex-basis: 300px;
    text-align: center;
    padding: 30px;
    border: 1px solid #222;
    margin: 10px;
}
</style>
