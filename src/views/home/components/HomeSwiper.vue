<template>
  <div>
    <swiper>
      <swiper-item v-for="item in banners" :key="item.title">
        <a :href="item.link">
          <img :src="item.image" alt="" />
        </a>
      </swiper-item>
    </swiper>
  </div>
</template>

<script>
import { Swiper, SwiperItem } from "components/common/swiper";
export default {
  name: "HomeSwiper",
  components: { Swiper, SwiperItem },
  data() {
    return {};
  },
  props:{
     banners:{
         type:Array,
         default(){
             return [];
         }
     }
  },
  mounted() {},

  methods: {},
};
</script>

<style lang="scss" scoped></style>
