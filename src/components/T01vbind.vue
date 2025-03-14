<script>
  export default {
    name: 'T01vbind',
    components : {},
    data() {
      return {
        var_class: "myClassName1",
        var_myUrl: "https://picsum.photos/300/200",
        var_size: "24px"        
    }
   }
  }  
</script>

<template lang="">
  <div v-bind:class="var_class">
    <div v-bind:style="{ fontSize: var_size }">
      <p>The browser finds the 'src' attribute value from the Vue instance with the use of 'v-bind'.</p>
      <img v-bind:src="var_myUrl">
    </div>
  </div>
</template>

<style>
  .myClassName1{
    background-color: red;
  }
  .myClassName2{
    background-color: rgb(77, 83, 251);
    padding: 40px;
  }
</style>