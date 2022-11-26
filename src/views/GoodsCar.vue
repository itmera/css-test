<template>
  <div class="bg-gray-300 h-screen p-2">
    <div class="bg-white rounded-lg p-2">
      <div class="flex py-4 gap-1">
        <input type="radio" class="w-4 h-6" name="" id="" />
        <p class="h-6 leading-6 text-lg">天猫会员店</p>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-6 h-6"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M8.25 4.5l7.5 7.5-7.5 7.5"
          />
        </svg>
      </div>
      <div class="flex h-4 justify-between text-sm">
        <p class="leading-4 text-gray-600">开通会员才可以购买店内商品</p>
        <div class="flex text-red-500">
          <span class="leading-4">去开通</span>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-6 h-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M8.25 4.5l7.5 7.5-7.5 7.5"
            />
          </svg>
        </div>
      </div>
      <!-- 商品列表 -->
      <div class="grid grid-cols-1 divide-y divide-gray-300">
        <div
          class="flex p-2 gap-2 items-center justify-between"
          v-for="(a, i) in dataList"
          :key="i"
        >
          <input type="radio" class="w-4 h-6" name="" id="" />
          <div class="w-20 h-20">
            <img :src="a.img" class="w-[98%]" alt="" />
          </div>
          <div class="flex-1 flex flex-col justify-start">
            <p class="flex-1 text-base">{{ a.title }}</p>
            <p class="h-6 text-red-300">限购{{ a.xgnum }}件</p>
            <div class="h-6 flex justify-between items-end align-bottom">
              <div class="flex-1 space-x-1">
                <span class="text-yellow-500">¥{{ a.price }}</span>
                <span class="text-xs">{{ a.zlnum }}kg</span>
              </div>
              <div class="flex justify-center border-gray-300">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                  class="w-5 h-5 border"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M18 12H6"
                  />
                </svg>

                <p class="h-5 leading-5 px-2 border-y text-sm">
                  {{ a.salenum }}
                </p>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                  class="w-5 h-5 border"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M12 6v12m6-6H6"
                  />
                </svg>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="h-16"></div>
    <div
      class="fixed h-14 w-full bg-white inset-x-0 bottom-0 flex justify-between"
    >
      <div class="flex-1 flex justify-around">
        <div class="flex items-center flex-col self-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-6 h-6 text-blue-500"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M20.25 8.511c.884.284 1.5 1.128 1.5 2.097v4.286c0 1.136-.847 2.1-1.98 2.193-.34.027-.68.052-1.02.072v3.091l-3-3c-1.354 0-2.694-.055-4.02-.163a2.115 2.115 0 01-.825-.242m9.345-8.334a2.126 2.126 0 00-.476-.095 48.64 48.64 0 00-8.048 0c-1.131.094-1.976 1.057-1.976 2.192v4.286c0 .837.46 1.58 1.155 1.951m9.345-8.334V6.637c0-1.621-1.152-3.026-2.76-3.235A48.455 48.455 0 0011.25 3c-2.115 0-4.198.137-6.24.402-1.608.209-2.76 1.614-2.76 3.235v6.226c0 1.621 1.152 3.026 2.76 3.235.577.075 1.157.14 1.74.194V21l4.155-4.155"
            />
          </svg>
          <p>客服</p>
        </div>
        <div class="flex items-center flex-col self-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-6 h-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M13.5 21v-7.5a.75.75 0 01.75-.75h3a.75.75 0 01.75.75V21m-4.5 0H2.36m11.14 0H18m0 0h3.64m-1.39 0V9.349m-16.5 11.65V9.35m0 0a3.001 3.001 0 003.75-.615A2.993 2.993 0 009.75 9.75c.896 0 1.7-.393 2.25-1.016a2.993 2.993 0 002.25 1.016c.896 0 1.7-.393 2.25-1.016a3.001 3.001 0 003.75.614m-16.5 0a3.004 3.004 0 01-.621-4.72L4.318 3.44A1.5 1.5 0 015.378 3h13.243a1.5 1.5 0 011.06.44l1.19 1.189a3 3 0 01-.621 4.72m-13.5 8.65h3.75a.75.75 0 00.75-.75V13.5a.75.75 0 00-.75-.75H6.75a.75.75 0 00-.75.75v3.75c0 .415.336.75.75.75z"
            />
          </svg>
          <p>店铺</p>
        </div>
        <div class="flex items-center flex-col self-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-6 h-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M11.48 3.499a.562.562 0 011.04 0l2.125 5.111a.563.563 0 00.475.345l5.518.442c.499.04.701.663.321.988l-4.204 3.602a.563.563 0 00-.182.557l1.285 5.385a.562.562 0 01-.84.61l-4.725-2.885a.563.563 0 00-.586 0L6.982 20.54a.562.562 0 01-.84-.61l1.285-5.386a.562.562 0 00-.182-.557l-4.204-3.602a.563.563 0 01.321-.988l5.518-.442a.563.563 0 00.475-.345L11.48 3.5z"
            />
          </svg>
          <p>收藏</p>
        </div>
      </div>
      <button class="bg-yellow-400 w-24 text-white">加入购物车</button>
      <button class="bg-red-400 w-24 text-white">马上抢</button>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
const dataList = ref([
  {
    img: "src/assets/images/07/02.jpg",
    title: "仁和潽园有机爱心红糖姜茶黑糖姜枣茶生姜红糖水大姨妈月女友独立小包装",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/03.webp",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/04.webp",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/08.jpg",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/05.webp",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/06.webp",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/07.jpg",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/09.jpg",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/02.jpg",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/03.webp",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/04.webp",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/08.jpg",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/05.webp",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/06.webp",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/07.jpg",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
  {
    img: "src/assets/images/07/09.jpg",
    title: "商品名字",
    xgnum: 10,
    price: 19.9,
    zlnum: 1.4,
    salenum: 2,
  },
]);
</script>

<style scoped></style>
