<template>
  <h1>jao</h1>
</template>

<script>
export default {
  props: {
    id: {
      type: Number,
      default: 2
    }
  },
  mounted() {
    console.log(this.$route.params.id)
  }
}
</script>

<style></style>
