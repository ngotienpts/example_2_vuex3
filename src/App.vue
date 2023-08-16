<script>
import Navbar from "./components/Navbar.vue";
import TodoList from "./components/TodoList.vue";
import AddTodo from "./components/AddTodo.vue";
export default {
    name: "App",
    components: {
        Navbar,
        TodoList,
        AddTodo,
    },
};
</script>
<template>
    <div id="app">
        <Navbar />
        <AddTodo />
        <TodoList />
    </div>
</template>
<style></style>
