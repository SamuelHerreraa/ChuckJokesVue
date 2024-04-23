<template>
    <div class="card" style="width: 18rem;">
      <img :src="iconUrl" class="card-img-top" alt="Chuck Norris">
      <div class="card-body">
        <p class="card-text">{{ value }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ChuckCard',
    props: {
      iconUrl: String,
      value: String
    }
  }
  </script>
  
  <style scoped>
  .card {
    margin-bottom: 20px;
  }
  </style>  