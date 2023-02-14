<script setup>
import AdsComp from './components/AdsComp.vue';
import NavComp from './components/NavComp.vue';
import HeaderComp from './components/HeaderComp.vue';
import AdviceComp from './components/AdviceComp.vue';
</script>

<template>
    <AdsComp />
    <!-- === --- === --- === Nav Start === --- === --- === --- ===-->
    <NavComp/>
    <!-- == -- == -- == -- == Header start -- == -- == -- == -- ==  -->
    <HeaderComp/>
    <!-- -- == == -- -- == == -- -- Main Start -- -- == == -- -- == == -- -- == == -->
    <main>
        <!-- -- == == -- -- == == -- -- Advice section Start -- -- == == -- -- == == -- -- == == -->
        <AdviceComp />
    </main>
</template>


<style scoped>

</style>
