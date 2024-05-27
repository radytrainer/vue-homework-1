<template>
  <li class="list-group-item">Employee name: <span class="badge bg-primary rounded-pill">{{ name }}</span></li>
</template>

<script>
export default {
    props: {
        name: String
    }
}
</script>

<style>

</style>