<template>
  
  <Child />

  <h3>Parent beforeCreate</h3>
  <h3>Parent created</h3>
  <h3>Parent beforeMount</h3>
  <h4>Child beforeCreate</h4>
  <h4>Child created</h4>
  <h4>Child beforeMount</h4>
  <h4>Child mounted</h4>
  <h4>Child beforeUpdate</h4>
  <h4>Child updated</h4>
  <h4>Child beforeUnmount</h4>
  <h4>Child unmounted</h4>
  <h3>Parent beforeUpdate</h3>
  <h3>Parent updated</h3>
  <h3>Parent beforeUnMount</h3>
  <h3>Parent unmounted</h3>

</template>

<script>
import Child from './components/Child.vue';

export default {
  name: 'App',
  components: {
    Child
  },
  beforeCreate: ()=>{
    console.log("Parent beforeCreate");
  },
  created: ()=>{
    console.log("Parent created");
  },
  beforeMount: ()=>{
    console.log("Parent beforeMount");
  },
  mounted: ()=>{
    console.log("Parent mounted");
  },
  beforeUpdate:()=>{
    console.log("Parent beforeUpdate");
  },
  updated:()=>{
    console.log("Parent updated");
  },
  beforeUnmount:()=>{
    console.log("Parent beforeUnmount");
  },
  unmounted:()=>{
    console.log("Parent unmounted");
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  max-width: 600px;
  margin: auto;
}

h3{
  background-color: #20cf8c;
  padding: 10px;
}

h4{
  background-color: #f59134;
  padding: 10px;
}

h1{
  font-weight: 800;
}

</style>
