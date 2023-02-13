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
                    <a href="#!"><i class="fa-solid fa-magnifying-glass nav__search"></i></a>
                    <li v-for="navLink in navLinks" class="nav__item" @click="navItem">
                        <a href="#!" class="nav__link">{{ navLink.name }} <i class="icon" :class="navLink.icon"></i></a>
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
    position: relative;
    transition: 1.5s;
}
.nav__item::before {
    content: '';
    position: absolute;
    bottom: 0;
    background: #DD4053;
    width: 0;
    height: 3px;
    display: flex;
    align-items: end;
    transition: 1.5s;
    top: 40px;
    transition: 500ms;
}
.nav__item:hover::before {
    width: 100%;
}
.nav__item:hover .icon {
    transition: 500ms;
    transform: rotateZ(180deg);
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
    font-size: 12px;
}
.nav__search {
    color: #343434;
}
</style>