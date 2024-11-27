<template lang="">
  <div>
    <h1>Example: 'v-bind' with Conditional Background Color</h1>

    <p>The browser sets the background color with 'hsl()' based on the value of 'bgVal' in the Vue instance.</p>

    <div id="app">
      <div v-bind:style="{ backgroundColor: isImportant ? 'lightcoral' : 'lightgray' }">Importance based on background color</div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'T01vbind',
    components : {},
    data() {
      return {
        isImportant: true
    }
   }
  }  
</script>

<style>
  
</style>