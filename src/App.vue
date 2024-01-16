<template><StudentsList /></template>

<script>
import StudentsList from "./components/Students.vue";

export default {
  name: "App",
  components: {
    StudentsList,
  },
};
</script>

<style>
#app {
  color: #2c3e50;
  margin-top: 60px;
}

ul {
  list-style: none;
}
</style>
