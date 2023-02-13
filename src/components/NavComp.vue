<script setup>
import { reactive, ref } from 'vue'
const navLinks = ref([
    {
        name: 'Отели',
        icon: "fa-solid fa-caret-down",
    },
    {
        name: 'Страны',
        icon: "fa-solid fa-caret-down",
    },
    {
        name: 'Авиа',
        icon: "fa-solid fa-caret-down",
    },
    {
        name: 'Каталог туров',
    },
    {
        name: 'Агентам',
        icon: "fa-solid fa-caret-down",
    },
    {
        name: 'О нас',
        icon: "fa-solid fa-caret-down",
    },
    {
        name: 'Блог',
    },
    {
        name: 'FAQ',
    },
    {
        name: 'Контакты',
    },

])

</script>
<template>
    <nav class="nav">
        <div class="container">
            <div class="nav__content">
                <ul class="nav__list">
                    <i class="fa-solid fa-magnifying-glass"></i>
                    <li v-for="navLink in navLinks" class="nav__item">
                        <a href="#!" class="nav__link">{{ navLink.name }}</a>
                        <i :class="navLink.icon"></i>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>


<style scoped>
.nav {
    border-top: 1px solid #D0D0D0;
}

.nav__list {
    display: flex;
    justify-content: space-between;
}

.nav__item {
    display: flex;
    align-items: center;
}

.nav__content {
    margin-top: 29px;
}

.nav__link {
    font-weight: 400;
    font-size: 15px;
    color: #616161;
}

.nav__item i {
    color: #C4C4C4;
    margin-left: 8px;
    font-size: 10px;
}
</style>