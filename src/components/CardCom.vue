<template>
  <div class="card">
    <img class="card-img-top" :src="data.image" alt="Card image" />
    <div class="card-body">
      <h4 class="card-title">{{ data.name }}</h4>
      <p class="card-text">{{ data.description }}</p>
    </div>
  </div>
</template>

<script>
export default {
    props: {
        data: Object
    }
};
</script>

<style>
</style>