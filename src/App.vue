<script>
export default {
  data() {
    return {
      name: "john doe",
      status: "active",
      statusNow: "active",
      tasks: ["Task one", "Task two", "Task three"],
      link: "https://google.com",
    };
  },
};
</script>

<template>
  <h1>Vue job {{ name }}</h1>
  <h4 v-if="status">the user is active {{ name }}</h4>
  <h4 v-else-if="status === pending">the user is pending</h4>
  <h4 v-else>the user is active</h4>

  <h2>Tasks:</h2>
  <ul>
    <li v-for="task in tasks" key="task">{{ task }}</li>
  </ul>

  <a v-bind:href="link">Click for google</a>
  <!-- short way -->
  <a :href="link">Click for google</a>
</template>

<style scoped>
h1 {
  background-color: aqua;
  color: brown;
}
</style>
