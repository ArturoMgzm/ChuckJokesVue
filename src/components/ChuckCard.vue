<template>
    <div class="card mb-3">
      <img :src="iconUrl" class="card-img-top" alt="Chuck Norris">
      <div class="card-body">
        <p class="card-text">{{ value }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ChuckCard',
    props: ['iconUrl', 'value']
  }
  </script>
  
  <style scoped>
  .card {
    border: 1px solid #FFFFFF;
    border-radius: 0.25rem;
    margin-bottom: 25px;
  }
  
  .card-img-top {
    height: 200px;
    object-fit: cover;
    border-top-left-radius: calc(0.25rem - 1px);
    border-top-right-radius: calc(0.25rem - 1px);
  }
  
  .card-body {
    padding: 1rem;
  }
  
  .card-text {
    margin: 0;
  }
  </style>