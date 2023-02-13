<script setup>
import { reactive, ref } from 'vue'
const prices = ref([
    {
        name: 'USD',
        maney: '28,90'
    },
    {
        name: 'EUR',
        maney: '35,00'
    }
]);
</script>

<template>
    <div class="ads">
        <div class="ads__container">
            <div class="ads__content d-flex align-items-center justify-content-between">
                <div class="ads__logo">
                    <a href="#!"><img src="../img/logo/logo (1) 1 (1).svg" alt=""></a>
                </div>
                <div class="dash"><span></span></div>
                <div class="ads__languages">
                    <ul class="ads__list">
                        <li class="ads__item"><a href="#!" class="ads__link">UZ</a></li>
                        <li class="ads__item"><a href="#!" class="ads__link">RU</a></li>
                    </ul>
                </div>
                <div class="dash"><span></span></div>
                <div class="ads__money-box">
                    <div class="money" v-for="price in prices">{{ price.name }} {{ price.maney }}</div>
                </div>
                <div class="dash"><span></span></div>
                <div class="ads__icons d-flex">
                    <a href="#!" class="ads__icon"><i class="fa-brands fa-facebook-f"></i></a>
                    <a href="#!" class="ads__icon"><i class="fa-brands fa-instagram"></i></a>
                    <a href="#!" class="ads__icon"><i class="fa-brands fa-youtube"></i></a>
                </div>
                <div class="dash"><span></span></div>
                <div class="ads__call-box d-flex">
                    <div class="ads__numbers">
                        <a href="#!" class="phone__number d-flex">044-537-20-07</a>
                        <a href="#!" class="phone__number d-flex">068-537-20-07</a>
                    </div>
                    <div class="ads__call-box-icon">
                        <img src="../img/logo/Group (6).svg" alt="">
                    </div>
                </div>
                <div class="dash"><span></span></div>
                <div class="ads__search d-flex">
                    <div class="search__box">
                        <p>Maistra ONLINE</p>
                        <button><img src="../img/logo/Group (7).svg" alt=""></button>
                    </div>
                    <div class="search__box">
                        <p>ТУРЫ ONLINE</p>
                        <button><img src="../img/logo/Frame 18 (1).svg" alt=""></button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.ads {
    margin-top: 17px;
}

.ads__container {
    max-width: 1237px;
    width: 100%;
    margin: 0 auto;
    padding: 0 15px;
    color: #393939;
}

.search__box button {
    border: none;
    background: var(--button-background);
    padding: 16px;
    border-radius: 2px;
    cursor: pointer;
}

.search__box:last-of-type button {
    background: #4AD295;
    padding: 16.5px 18px;
}

.search__box:last-of-type {
    margin-left: 30px;
}

.search__box {
    height: 55px;
    display: flex;
    align-items: center;
    justify-content: center;
    background: #EFF3F6;
    border-radius: 2px;
}

.search__box p {
    padding: 0 20px;
    font-weight: 600;
    color: #373737;
}

.ads__numbers {
    margin-right: 7px;
    row-gap: 5px;
    font-weight: 700;
    font-size: 16px;
    color: #393939;
}

.ads__icons {
    column-gap: 15px;
    display: flex;
    align-items: center;
}

.ads__icon i {
    color: #E2E2E2;
    font-size: 18px;
}

.ads__icon:nth-last-of-type(2) i {
    color: #E2E2E2;
    font-size: 20px;
}


.dash {
    position: relative;
}

.dash span {
    position: absolute;
    height: 40px;
    width: 1px;
    background: #E2E2E2;
    top: -19px;
}

.ads__link {
    color: #1f1f1f;
}

.money {
    color: #393939;
    font-size: 15px;
}

.phone__number {
    color: #393939;
}
</style>