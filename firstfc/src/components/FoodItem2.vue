<template>
  <div class="Foie Gras">
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


<style>
.Foie Gras{
     border: dashed black 1px;
    display: inline-block;
    margin: 10px;
    padding: 10px;
    background-color: rgba(217, 206, 252, 0.38);
  }  
  </style>