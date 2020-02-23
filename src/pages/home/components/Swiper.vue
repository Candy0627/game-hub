<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
            <swiper-slide v-for="item in swiperList" :key="item.id">
                <img class="swiper_img" :src="item.imgUrl" alt="">
            </swiper-slide>
            <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
    </div>
</template>

<script>
export default {
    name:'homeSwiper',
    data () {
        return {
            swiperOption:{
                pagination:'.swiper-pagination',
                loop:true
            },
            swiperList:[{
                id:'001',
                imgUrl:'../../../../static/images/banner01.jpg'
            },{
                id:'002',
                imgUrl:'../../../../static/images/banner02.jpg'
            },{
                id:'003',
                imgUrl:'../../../../static/images/banner03.jpg'
            }]
        }
    }
}
</script>

<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active
        background: #fff !important
.wrapper
    width:100%
    overflow: hidden
    height:0
    padding-bottom:39.1%
    background: #eee
    .swiper_img
        width: 100%
</style>