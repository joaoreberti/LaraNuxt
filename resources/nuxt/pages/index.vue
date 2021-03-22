<template>
  <v-row column justify="center" align="center">
    <div>{{ this.$store.state.user.name }}</div>
  </v-row>
</template>

<script>
export default {
  data() {
    return {}
  }
}
</script>
