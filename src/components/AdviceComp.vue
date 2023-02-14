<script>

</script>

<template>
    <section class="advice__section">
        <div class="container d-flex">
            <div class="advice__left">
                <div class="advice__title">ВАШ ТУРОПЕРАТОР ВЫСОКОГО<br> УРОВНЯ ОБСЛУЖИВАНИЯ.</div>
                <div class="advice__left-text">
                    Откройте мир путешествий заново.
                </div>
                <div class="advice__left-btns">
                    <button class="advice__left-btn">Что мы предлагаем?</button>
                    <button class="advice__left-btn">Консультация</button>
                </div>
            </div>
            <div class="advice__right d-flex">
                <div class="advice__right-img">
                    <div class="advice__right-img-box">
                        <img src="../img/logo/Group 153.svg" alt="">
                    </div>
                    <div class="advice__right-img-box">
                        <img src="../img/logo/Group 152.svg" alt="">
                    </div>
                    <div class="advice__right-img-box">
                        <img src="../img/logo/Vector (2).svg" alt="">
                    </div>
                </div>
                <p class="text">
                    ИНДИВИДУАЛЬНЫЙ ПОДХОД 
                    <br> КОНСЬЕРЖ-СЕРВИС 
                    <br>ОТДЫХ ПРЕМИУМ-КЛАССА
                </p>
            </div>
        </div>
    </section>
</template>

<style scoped>
.advice__section {
    background: #F8F8F8;
}

.advice__title {
    font-weight: 600;
    font-size: 30px;
    color: #1D1D1D;
    margin: 30px 0 15px 0;
}

.advice__right {
    margin-left: 166px;
}

.advice__left-text {
    font-size: 16px;
    font-weight: 600;
    color: #777777;
}

.advice__left-btn {
    padding: 15px 44px;
    background: #F8F8F8;
    border: 2px solid #969696;
    border-radius: 2px;
    color: #BDBDBD;
    font-weight: 700;
    font-size: 16px;
    cursor: pointer;
}

.advice__left-btn:first-of-type {
    background: #BDBDBD;
    color: #FFFFFF;
    border: none;
}
.advice__left-btns {
    margin: 20px 0 35px 0;
    column-gap: 30px;
    display: flex;
}

.advice__right-img-box {
    background: url(../img/logo/box.svg) no-repeat center center / cover;
    width: 45px;
    height: 45px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.advice__right-img {
    column-gap: 20px;
}
.text {
    line-height: 66px;
    margin-top: 27px;
}
.advice__right-img-box {
    margin-top: 20px;
    margin-right: 20px;
}
.advice__right-img-box:first-of-type {
    margin-top: 37px;
}
</style>