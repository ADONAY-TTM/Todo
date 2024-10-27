<template>
  <h1>{{ wellcomeMsg }}</h1>
  <input id="ideaInput" type="text" ref="idea" placeholder="Things Todo" />
  <button @click="handleNewTodo">Add</button>
  <Todo />
  <Done />
</template>

<script>
import Todo from "./components/Todo.vue";
import Done from "./components/Done.vue";

export default {
  name: "App",
  components: {
    Todo,
    Done,
  },
  methods: {
    handleNewTodo() {
      console.log("ToDo");
    },
  },

  data() {
    return {
      wellcomeMsg: "Welcome, What's On Your Mind Today",
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
h1 {
  border-bottom: 1px solid #ddd;
  display: inline-block;
  padding-bottom: 10px;
}
#ideaInput {
  margin: 20px;
  padding: 10px;
}
button {
  background-color: #04aa6d;
  border-radius: 9px;
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
}
input[type="text"] {
  width: 200px;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
  font-size: 16px;
  color: #333333;
  background-color: #f9f9f9;
  transition: border-color 0.3s ease;
}

input[type="text"]:focus {
  border-color: #007bff;
  outline: none;
  background-color: #fff;
  box-shadow: 0 0 5px rgba(0, 123, 255, 0.3);
}
</style>
