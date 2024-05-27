<template>
  <div class="alert alert-success">
    <strong>User:</strong> {{ name }}
  </div>
</template>

<script>
export default {
    props: {
        name: String
    }
};
</script>

<style>
</style>