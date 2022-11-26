<template>
  <div class="bg-red-600 h-screen">
    <div class="h-20 flex justify-between items-center px-4">
      <div class="text-white">
        <p>每月零30元红包，一年零360元红包</p>
        <p class="text-xs text-gray-400 pt-1">
          花0.24元/天，预计每年可省2360元以上
        </p>
      </div>
      <button class="px-2 py-1 bg-orange-400 text-orange-700 rounded-xl">
        立即入会
      </button>
    </div>
    <div class="bg-white m-1 rounded-xl">
      <p class="pl-2 h-6 leading-6 my-2 text-red-400 text-sm">
        入会每月领30元红包
      </p>
      <!-- 领券列表 -->
      <div class="grid grid-cols-3 text-red-400 gap-2 px-1 my-2">
        <div
          class="bg-red-200 flex self-center items-center text-xs rounded-lg"
          v-for="(a, i) in 3"
          :key="i"
        >
          <div class="flex-1 p-1">
            <p class="text-2xl">￥{{ Math.floor(a * Math.random() * 20) }}</p>
            <p>满{{ (a * 99) / 2 }}可用</p>
            <p>每月可领一张</p>
          </div>
          <p
            class="w-8 h-full text-sm px-2 border-l border-dashed border-gray-500"
          >
            领取
          </p>
        </div>
      </div>
      <!-- 立减优惠 -->
      <p class="p-2 h-6 leading-6 mb-2 text-red-400">会员入会礼 限购一件</p>
      <div class="grid grid-cols-4 gap-2 pt-5 px-2">
        <div class="relative" v-for="(a, i) in dataList" :key="i">
          <img :src="a.img" class="w-[95%] rounded-lg" alt="" />
          <p class="text-red-400 text-xs text-center">
            新人价￥<span class="font-medium text-lg">{{ a.price }}</span>
          </p>
          <div class="absolute right-0 top-0">
            <p class="bg-red-600 w-7 h-6 text-xs text-red-100 text-center">
              立省<br />{{ a.lis }}
            </p>
            <p
              class="w-7 border-transparent border-[0.875rem] border-t-red-600"
            ></p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const dataList = ref([
  {
    img: "src/assets/images/07/02.jpg",
    price: 9.9,
    lis: 8,
  },
  {
    img: "src/assets/images/07/03.webp",
    price: 23.9,
    lis: 28,
  },
  {
    img: "src/assets/images/07/04.webp",
    price: 19.9,
    lis: 29,
  },
  {
    img: "src/assets/images/07/08.jpg",
    price: 29.9,
    lis: 36,
  },
  {
    img: "src/assets/images/07/05.webp",
    price: 9.9,
    lis: 8,
  },
  {
    img: "src/assets/images/07/06.webp",
    price: 23.9,
    lis: 28,
  },
  {
    img: "src/assets/images/07/04.webp",
    price: 19.9,
    lis: 29,
  },
  {
    img: "src/assets/images/07/03.webp",
    price: 29.9,
    lis: 36,
  },
  {
    img: "src/assets/images/07/06.webp",
    price: 9.9,
    lis: 8,
  },
  {
    img: "src/assets/images/07/05.webp",
    price: 23.9,
    lis: 12,
  },
  {
    img: "src/assets/images/07/04.webp",
    price: 19.9,
    lis: 19,
  },
  {
    img: "src/assets/images/07/08.jpg",
    price: 29.9,
    lis: 26,
  },
]);
</script>
