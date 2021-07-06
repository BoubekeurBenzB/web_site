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
    background-color: #17151a;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 10;
}
.menu {
    display: flex;
    list-style: none;
}
.menu-item {
    padding: 1rem;
    color: #babcc5;
    cursor: pointer;
}
.menu-item:hover {
    color: #f1f1f1;
}
.menu-item:last-child {
    margin-right: 5rem;
}
</style>