<template>
  <div class="wrapper">
    <h1>{{ message }}</h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: null,
    };
  },
  created() {
    this.message = this.$store.getters.getMessage;
  },
};
</script>

<style lang="scss" scoped>
h1 {
  color: green
}
</style>