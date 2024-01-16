<template>
  <div class="cards">
    <ul v-for="student in studentsList" :key="student.name">
      <li>
        <div>
          <p>Name:</p>
          <p>{{ student.name }}</p>
        </div>
        <div>
          <p>Age:</p>
          <p>{{ student.age }}</p>
        </div>
        <div>
          <p>Height:</p>
          <p>{{ student.height }}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
import { defineComponent } from "vue";
export default defineComponent({
  name: "StudentsList",
  setup() {
    const studentsList = [
      { name: "John", age: 20, height: 175 },
      { name: "Jane", age: 19, height: 165 },
      { name: "Bob", age: 21, height: 180 },
      { name: "Alice", age: 22, height: 170 },
      { name: "David", age: 23, height: 185 },
      { name: "Emily", age: 20, height: 160 },
      { name: "Frank", age: 22, height: 178 },
      { name: "Grace", age: 21, height: 172 },
    ];

    return {
      studentsList,
    };
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
