<template>
    <div>
        <home-menu></home-menu>
        <home-swiper></home-swiper>
    </div>
</template>

<script>
import HomeMenu from './components/Menu'
import HomeSwiper from './components/Swiper'
export default {
    name:'Home',
    components:{
        HomeMenu,
        HomeSwiper
    }
}
</script>

<style>

</style>