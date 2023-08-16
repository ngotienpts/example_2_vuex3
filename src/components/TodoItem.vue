<script>
export default {
    name: "TodoItem",
    props: ["todoProps"],
};
</script>
<template>
    <div :class="['todo-item', todoProps.completed ? ' is-completed' : '']">
        <div class="todo-item__action">
            <label :for="todoProps.id" class="todo-item__label">{{
                todoProps.title
            }}</label>
            <input
                type="checkbox"
                :name="todoProps.title"
                :id="todoProps.id"
                class="todo-item__input"
            />
        </div>
        <button class="todo-btn">Delete</button>
    </div>
</template>
<style scoped>
.todo-item {
    background-color: #a8dadc;
    padding: 10px;
    display: flex;
    align-items: center;
    gap: 20px;
    border-bottom: 1px solid #f1faee;
}
.is-completed {
    background-color: #e63946;
}
.todo-item:last-child {
    border-bottom: none;
}
.todo-item__action {
    flex: 1;
    display: flex;
    align-items: center;
}
.todo-item__label {
    flex: 1;
    color: #000;
}
.is-completed .todo-item__label {
    color: #fff;
}
.todo-item__input {
    flex-shrink: 0;
}
.todo-btn {
    cursor: pointer;
}
</style>
