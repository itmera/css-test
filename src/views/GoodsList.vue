<template>
  <div class="grid grid-cols-2 gap-2 p-2 bg-gray-300">
    <div
      v-for="(a, i) in dataList"
      :key="i"
      class="rounded-2xl relative bg-white"
    >
      <img :src="a.img" class="w-full rounded-t-xl" alt="" />
      <p class="h-9 leading-10 text-xl">{{ a.title }}</p>
      <div class="flex flex-wrap space-x-2 text-xs p-2">
        <p v-if="a.yunfeixian">
          <span class="bg-blue-500 text-white font-medium">享</span>
          <span class="text-blue-500 rounded-xl border px-1 border-blue-600"
            >退货运费险</span
          >
        </p>
        <p>
          <span class="rounded-xl border px-1 border-red-600 text-red-600">
            {{ a.huodong }}
          </span>
        </p>
      </div>
      <p class="text-red-500 leading-10 h-10 m-0 pl-4">
        活动价￥ <span class="text-2xl"> {{ a.price }}</span>
      </p>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const dataList = ref([
  {
    img: "src/assets/images/07/02.jpg",
    title: "Nubia手机",
    slogn: "月销1w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/03.webp",
    title: "大宝Sod蜜",
    slogn: "月销27w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/04.webp",
    title: "家用热水器",
    slogn: "月销9w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/08.jpg",
    title: "全麦素食饼干",
    slogn: "月销32w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/05.webp",
    title: "双胆速热水器",
    slogn: "月销6w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/06.webp",
    title: "西凤酒53度",
    slogn: "月销19w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/07.jpg",
    title: "三星手机A53",
    slogn: "月销2w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/09.jpg",
    title: "奥克斯空气炸锅",
    slogn: "月销3.5w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/02.jpg",
    title: "Nubia手机",
    slogn: "月销1w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/03.webp",
    title: "大宝Sod蜜",
    slogn: "月销27w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/04.webp",
    title: "家用热水器",
    slogn: "月销9w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/08.jpg",
    title: "全麦素食饼干",
    slogn: "月销32w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/05.webp",
    title: "双胆速热水器",
    slogn: "月销6w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/06.webp",
    title: "西凤酒53度",
    slogn: "月销19w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/07.jpg",
    title: "三星手机A53",
    slogn: "月销2w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
  {
    img: "src/assets/images/07/09.jpg",
    title: "奥克斯空气炸锅",
    slogn: "月销3.5w件",
    yunfeixian: true,
    huodong: "每300减30",
    price: 72.99,
  },
]);
</script>

<style scoped></style>
