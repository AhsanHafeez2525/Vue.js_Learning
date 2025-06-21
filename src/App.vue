<script>
export default {
  data() {
    return {
      name: "john doe",
    };
  },
};
</script>

<template>
  <h1>Vue job {{ name }}</h1>
</template>

<style scoped>
h1 {
  background-color: aqua;
  color: brown;
}
</style>
