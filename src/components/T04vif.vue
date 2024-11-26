<template>
  <div>
    <h1>Example with 'v-if' and 'v-else'</h1>

    <p>Try changing the 'typewritersInStock' value in the Vue instance from 'true' to 'false' and run the code again.</p>

    <div id="example04">
      <p v-if="typewritersInStock">
        in stock
      </p>
      <p v-else>
        not in stock
      </p>

      <p v-if="typewriterCount > 0">
        in stock
      </p>
      <p v-else>
        not in stock
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'T04vif',
  components : {},
  data() {
    return {
      typeWritersInStock: true,
      typewriterCount: 3
    }
  }
}
</script>

<style lang="css">
    #example04 {
      border: dashed black 1px;
      width: 130px;
      padding-left: 20px;
      font-weight: bold;
      background-color: lightgreen;
    }
</style>