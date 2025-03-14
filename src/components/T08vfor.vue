<template>
  <div>
    <h1>Example: 'v-for' to create li-tags</h1>

    <p>In this example 'v-for' creates an 'li' tag with the food name for each food item in the Vue instance array.</p>

    <div id="example08">
      <div>
        <ol>
          <li v-for="item in manyFoods">{{ item }}</li>
        </ol>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'T08vfor',
  components: {},
  data() {
    return {
      manyFoods: [
        'Burrito',
        'Salad',
        'Cake',
        'Soup',
        'Fish',
        'Pizza',
        'Rice'
      ]
    }
  }
}
</script>
<style lang="css">
  #example08 > div {
    border: dashed black 1px;
    width: 20%;
    padding: 10px;


  }
</style>