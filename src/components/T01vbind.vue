<script>
  export default {
    name: 'T01vbind',
    components : {},
    data() {
      return {
        url: "https://picsum.photos/200/100",
        size: "38px",
        class: "myClassName"
    }
   }
  }  
</script>

<template lang="">
  <div v-bind:class="class">
    <div v-bind:style="{ fontSize: size }">
      <p>The browser finds the 'src' attribute value from the Vue instance with the use of 'v-bind'.</p>
      <img v-bind:src="url">
    </div>
  </div>
</template>

<style>
.myClassName{
  background-color: red;
}
</style>