<template>
<div class="nav-container">
    <nav class="nav">
        <div class="logo">
            <h1>LOGO</h1>
        </div>
        <ul>
            <li>HOME</li>
            <li>ABOUT</li>
            <li>CONTACT</li>
        </ul>
    </nav>
</div>
</template>


<style scoped>
.nav-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
}
.nav {
    max-width: 1250px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
}
.nav ul {
    list-style: none;
    display: flex;
}
.nav li {
    margin: 0px 10px;
}
</style>