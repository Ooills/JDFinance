<template lang="html">
    <section :class="cname">
        <swiper :options="options" :not-next-tick="options.notNextTick">
            <swiper-slide v-for="item of items" :key="item.href">
                <router-link :to="{ name: item.href}">
                    <img :src="item.src" alt="">
                </router-link>
            </swiper-slide>
            <!--<div class="swiper-pagination" v-if="options.pagination"></div>-->
            <div class="swiper-pagination" v-if="options.pagination" slot="pagination"/>
            <div class="swiper-button-prev" slot="button-prev"></div>
            <div class="swiper-button-next" slot="button-next"></div>
            <!--<div class="swiper-scrollbar" slot="scrollbar"></div>-->
        </swiper>
    </section>
</template>

<script>
    import {swiper,swiperSlide} from 'vue-awesome-swiper';
    export default {
        name: "slider",
        components: {
            swiper,
            swiperSlide
        },
        props: {
            cname: {
              type: String,
              default: ''
            },
            options: {
                type: Object,
                default() {
                    return {
                       autoplay: true,
                       loop:true,
                       pagination: {
                           el: '.swiper-pagination'
                       },
                       notNextTick: false
                    }
                }
            },
            items: {
                type: Array,
                default() {
                    return []
                }
            }
        }

    }
</script>

<style scoped>
    @import "~swiper/dist/css/swiper.css";
</style>