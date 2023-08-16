<script>
export default {
    name: "AddTodo",
};
</script>
<template>
    <div class="form-group">
        <form class="form-add">
            <input type="text" class="form-text" />
            <input type="submit" value="Add" class="form-submit" />
        </form>
    </div>
</template>
<style scoped>
.form-group {
    background-color: #a8dadc;
}
.form-add {
    display: flex;
    align-items: center;
}
.form-text {
    height: 48px;
    flex: 10;
    padding: 10px;
    background-color: transparent;
    font-size: 16px;
    border: 0;
    outline: none;
    color: #000;
}
.form-submit {
    background-color: #e63946;
    height: 48px;
    flex: 2;
    border: 0;
    outline: none;
    color: #fff;
    font-size: 16px;
}
.form-submit:hover {
    background-color: #fa2f40;
    cursor: pointer;
}
</style>
