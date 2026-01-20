<template>
  <div class="food-card">
    <h2>{{ name }}</h2>
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: 'Foie Gras',
      message: 'It is tasty as well'
    }
  }
};
</script>

<style scoped>
.food-card {
  border: dashed black 1px;
  display: inline-block;
  margin: 10px;
  padding: 10px;
  background-color: rgba(126, 69, 166, 0.55);
}
</style>