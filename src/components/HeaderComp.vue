<script setup>
import { reactive } from 'vue';
const headerBg = reactive([
    { img: '../img/header-bg2.png' },
])
const iconClick = (pressed) => {
    
}

// function key() 

</script>
<template>
    <header class="header">
        <img src="../img/header-bg.png" alt="" class="header__bg" :src="headerbg" v-for="headerbg in headerBg">
        <div class="header__content">
            <div class="container">
                <div class="header__text">
                    <p>От 300 € за сутки</p>
                </div>
                <h1 class="header__title">
                    новый эко-отель mastila<br> на о. хвар в Хорватии
                </h1>
                <div class="header__btn">
                    <button class="btn">Подробнее</button>
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped>
.header {
    position: relative;
    min-height: 490px;
    margin-top: 23.5px;
    display: flex;
}

.header__bg {
    position: absolute;
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.header__content {
    position: relative;
    background: linear-gradient(180deg, rgba(0, 0, 0, 0.1) 14.37%, rgba(0, 0, 0, 0.8) 100%);
    flex-grow: 1;
}

.header__title {
    text-transform: uppercase;
    font-weight: 500;
    font-size: 45px;
    line-height: 55px;
    color: #FFFFFF;
    margin-bottom: 40px;
}

.header__text p {
    font-weight: 600;
    font-size: 24px;
    color: #FFFFFF;
}

.header__text {
    border: 1px solid #FFFFFF;
    width: 249px;
    height: 45px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 104px 0 16px 0;
}

.btn {
    padding: 18px 85px;
    border: none;
    background: rgba(255, 255, 255, 0.25);
    color: #FFFFFF;
    transition: 300ms;
    font-weight: 700;
    font-size: 16px;
    cursor: pointer;
    border-radius: 2px;
}
.btn:hover {
    background: rgba(255, 255, 255, 0.556);
    transition: 300ms;
}
</style>