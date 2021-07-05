<template>
    <div class="navbar">
        <ul class="menu">
            <li class="menu-item">About</li>
            <li class="menu-item">Skills</li>
            <li class="menu-item">Experience</li>
            <li class="menu-item">Portfolio</li>
            <li class="menu-item">Contact</li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'Navbar'
}
</script>

<style lang="scss" scoped>
.navbar {
    display: flex;
    justify-content: flex-end;
    align-items: center;
    background-color: #333;
}
.menu {
    display: flex;
    list-style: none;
}
.menu-item {
    padding: 10px;
    color: #f1f1f1;
}
.menu-item:last-child {
    margin-right: 2rem;
}
</style>