<template>
  <div class="hello">
    <h1>VueJs component LIFE CYCLE</h1>
    The life cycle is represented visually bellow.
  </div>
</template>

<script>
export default {
  name: 'ChildComp',
  props: {
    msg: String
  },
  beforeCreate: ()=>{
    console.log("Child beforeCreate");
  },
  created: ()=>{
    console.log("Child created");
  },
  beforeMount: ()=>{
    console.log("Child beforeMount");
  },
  mounted: ()=>{
    console.log("Child mounted");
  },
  beforeUpdate:()=>{
    console.log("Child beforeUpdate");
  },
  updated:()=>{
    console.log("Child updated");
  },
  beforeUnmount:()=>{
    console.log("Child beforeUnmount");
  },
  unmounted:()=>{
    console.log("Child unmounted");
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
