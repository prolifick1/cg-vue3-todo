<template>
  <h1>vue3 todo app</h1>
  <form @submit.prevent="addNewTodo">
    <label for="">New Todo</label>
    <input type="text" name="new todo" />
    <button>Add New Todo</button>
  </form>
</template>

<script>
export default {
  setup() {
    function addNewTodo() {
      console.log(`form was submitted`);
    }
    return {
      addNewTodo,
    };
  },
};
</script>

<style>
body {
  font-family: sans-serif;
  padding-top: 1em;
  padding-bottom: 1em;
  font-size: 2em;
  width: 80%;
  margin: 0 auto;
}
input,
textarea,
button,
p,
div,
section,
article,
select {
  display: "block";
  width: 100%;
  font-family: sans-serif;
  font-size: 1em;
  margin: 0.5em;
}
.todo {
  cursor: pointer;
}
.done {
  text-decoration: line-through;
}
</style>
