<template>
  <div class="bg-gray-300">
    <div class="h-12"></div>
    <div class="bg-white m-1 rounded-xl">
      <p class="pl-2 h-8 leading-8 text-lg mb-2">已购商品</p>
      <div
        class="flex justify-between text-xs border-b m-2 pb-2 border-solid border-gray-300"
        v-for="(a, i) in dataList"
      >
        <img :src="a.img" alt="" class="w-20 h-20" />
        <div class="flex-1 mx-2 flex justify-between flex-col">
          <p class="text-lg">{{ a.title }}</p>
          <p class="text-gray-400">{{ a.comp }}</p>
          <p class="text-gray-400">{{ a.dpnum }}人已点评</p>
        </div>
        <div class="flex flex-col justify-between items-end">
          <p
            v-if="a.isbuy"
            class="w-8 text-center bg-orange-200 text-orange-400"
          >
            已买
          </p>
          <button class="border border-gray-300 rounded-2xl py-1 px-2 flex">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="w-4 h-4 pr-1"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M7.5 8.25h9m-9 3H12m-9.75 1.51c0 1.6 1.123 2.994 2.707 3.227 1.129.166 2.27.293 3.423.379.35.026.67.21.865.501L12 21l2.755-4.133a1.14 1.14 0 01.865-.501 48.172 48.172 0 003.423-.379c1.584-.233 2.707-1.626 2.707-3.228V6.741c0-1.602-1.123-2.995-2.707-3.228A48.394 48.394 0 0012 3c-2.392 0-4.744.175-7.043.513C3.373 3.746 2.25 5.14 2.25 6.741v6.018z"
              />
            </svg>
            我要点评
          </button>
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
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/03.webp",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/04.webp",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/08.jpg",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/05.webp",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/06.webp",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/07.jpg",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/09.jpg",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/02.jpg",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/03.webp",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/04.webp",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/08.jpg",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/05.webp",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/06.webp",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/07.jpg",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
  {
    img: "src/assets/images/07/09.jpg",
    title: "商品名字",
    comp: "品牌",
    dpnum: 37,
    isbuy: true,
  },
]);
</script>

<style scoped></style>
