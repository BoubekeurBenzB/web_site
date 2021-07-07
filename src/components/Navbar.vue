<template>
    <div class="navbar">
        <div class="icon-toggle" @click="toggleMenu">
            <i class="fas fa-bars"></i>
        </div>
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
    name: 'Navbar',

    methods: {
        toggleMenu() {
            const menu = document.querySelector('.menu');

            menu.classList.toggle('menu-active');
        }
    }
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
.icon-toggle {
    display: none;
    color: #babcc5;
    cursor: pointer;
    font-size: 1.5rem;
    padding: 1rem;
    margin-right: 1rem;
}
.menu {
    display: flex;
    list-style: none;
}
.menu-item {
    font-weight: bold;
    text-transform: uppercase;
    padding: 1rem;
    color: #babcc5;
    cursor: pointer;
}
.item-active,
.menu-item:hover,
.icon-toggle:hover {
    color: #f1f1f1;
}
.menu-item:last-child {
    margin-right: 3rem;
}

/** responsive */

/** tablet & Ipad */
@media screen and (max-width: 1024px) {
    .icon-toggle {
        display: block;
    }
    .menu {
        display: none;
    }
    .menu-active {
        background-color: #17151a;
        border-top: 1px solid #babcc5;
        display: block;
        position: absolute;
        left: 0;
        right: 0;
        top: 3.9rem;
    }
    .menu-item {
        width: 100%;
        text-align: center;
    }
    .menu-item:last-child {
        margin-right: 0;
    }
}
</style>