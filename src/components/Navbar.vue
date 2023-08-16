<script>
export default {
    name: "Navbar",
};
</script>
<template>
    <div class="navbar">
        <div class="navbar-item">
            <div>Home</div>
            <div>Product</div>
            <div>About</div>
        </div>
        <div class="navbar-btn">
            <button>Login</button>
            <button>Logout</button>
        </div>
    </div>
</template>
<style scoped>
.navbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 30px;
    background-color: #1d3557;
    padding: 20px;
}
.navbar-item {
    flex: 10;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.navbar-btn {
    flex: 2;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.navbar-btn button {
    cursor: pointer;
}
</style>
