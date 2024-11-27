<template>
  <div>
    <h1>Example: Right Mouse Button Event</h1>

    <div id="example25">
      <div v-on:click.right="changeColor" v-bind:style="{ backgroundColor:'hsl('+bgColor+',80%,80%)' }">
        <p>Press right mouse button here.</p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      bgColor : 0
    }
  },
  methods: {
    changeColor() {
      this.bgColor+=50;
    }
  }
}
</script>
<style lang="css">
  #example25 {
    border: black dashed 1px;
    width: 200px;
    padding: 20px;
  }
  #example25 > div {
    width: 160px;
    padding: 20px;
    cursor: default;
    font-weight: bold;
  }
</style>