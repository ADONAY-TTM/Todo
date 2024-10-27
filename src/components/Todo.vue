<template>
  <div class="modalTodo">
    <h2>To-Do</h2>
    <li>Create a SPA website</li>
    <li>update the existing website</li>
  </div>
</template>
  
  <style scoped>
.modalTodo {
  margin: 30px;
  width: 600px;
  padding: 30px;
  background: white;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}
li {
  list-style-type: none;
  margin: 5px 0;
  padding: 10px;
  font-size: 16px;
  color: #333;
  background-color: #f0f0f0;
  border-radius: 5px;
}

li:hover {
  background-color: #11750380;
  cursor: pointer;
}
</style>
  