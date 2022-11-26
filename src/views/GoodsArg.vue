<template>
  <div class="bg-gray-700 w-full h-screen relative">
    <!-- 产品参数 -->
    <div class="absolute inset-x-0 h-[80%] bottom-0 top-15 bg-white">
      <h2 class="text-center text-xl my-4">产品参数</h2>
      <div class="gird divide-y-2 gap-3">
        <div
          v-for="(a, i) in dataList"
          :key="i"
          class="flex self-center items-center px-3 py-5 even:bg-gray-200"
        >
          <p class="w-32">{{ a.name }}</p>
          <p class="flex-1">{{ a.desc }}</p>
        </div>
      </div>
      <div class="h-16"></div>
      <button
        class="fixed inset-x-0 bottom-0 w-full h-12 text-xl text-gray-200 bg-red-500"
      >
        完成
      </button>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const dataList = ref([
  {
    name: "品牌",
    desc: "诗忆妃",
  },
  {
    name: "适用年龄",
    desc: "18-25周岁",
  },
  {
    name: "尺码",
    desc: "S (80-95F) M (95-105FF) L (105-115 斤）x(115-130斤〕",
  },
  {
    name: "颜色分类",
    desc: "217#白色上衣＋黑色裤子",
  },
  {
    name: "货号",
    desc: "S18CW4374",
  },
  {
    name: "上市年份季节",
    desc: "2019年夏季",
  },
  {
    name: "销售渠道类型",
    desc: "纯电商(只在线上销售）",
  },
  {
    name: "材质成分",
    desc: "其他100%",
  },
]);
</script>

<style scoped></style>
