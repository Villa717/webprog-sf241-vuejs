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
      name: 'Steak',
      message: 'It is tasty'
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
  background-color: lightcoral; /* Changed color so you can see the difference */
}
</style>

