<script>
import TodoItem from "./TodoItem.vue";

export default {
    name: "TodoList",
    components: {
        TodoItem,
    },
    data() {
        const todos = [
            {
                id: 1,
                title: "Viec 1",
                completed: false,
            },
            {
                id: 2,
                title: "Viec 2",
                completed: false,
            },
            {
                id: 3,
                title: "Viec 3",
                completed: false,
            },
        ];

        return { todos };
    },
};
</script>
<template>
    <div class="todo-list">
        <TodoItem v-for="todo in todos" :key="todo.id" :todoProps="todo" />
    </div>
</template>
<style scoped>
.todo-list {
    background-color: #457b9d;
    padding: 10px;
}
</style>
