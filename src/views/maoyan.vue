<template>
  <div class="bg-gray-100 h-screen pt-2">
    <div class="bg-gray-100">
      <h1 class="text-4xl text-red-200">猫眼</h1>
    </div>
    <div class="mb-1 px-2 h-10 bg-white flex justify-between items-center">
      <p class="w-1/4">上海</p>
      <div class="flex-1 flex justify-around">
        <p>热映</p>
        <p>待映</p>
      </div>
      <div class="w-1/4 flex flex-col items-end">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-6 h-6 text-red-400"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M15.75 15.75l-2.489-2.489m0 0a3.375 3.375 0 10-4.773-4.773 3.375 3.375 0 004.774 4.774zM21 12a9 9 0 11-18 0 9 9 0 0118 0z"
          />
        </svg>
      </div>
    </div>
    <div class="h-24 bg-blue-400 flex items-center pl-2 text-blue-200">
      <p class="w-1/2">
        电影红包派送<br />
        <span class="text-sm">十元观影红包免费抢</span>
      </p>
    </div>
    <!-- list -->
    <div class="px-2 border-t-2 gap-2">
      <div
        class="h-36 flex justify-between items-center border-b-2"
        v-for="(a, i) in dataList"
        :key="i"
      >
        <div class="w-1/4 relative">
          <img :src="a.img" class="rounded-xl" alt="" />
          <div class="absolute inset-0 flex justify-center items-center">
            <p class="text-xl text-white">▶️</p>
          </div>
        </div>
        <div class="flex-1 flex flex-col px-2 justify-between">
          <p class="text-lg">
            {{ a.title }}
            <span class="bg-blue-300 border text-white rounded-l text-xs"
              >3D</span
            >
            <span class="text-blue-300 border border-blue-300 rounded-r text-xs"
              >MAX</span
            >
          </p>
          <div class="text-gray-400">
            <p>
              <span class="text-orange-300">
                {{ a.wantsee }}
              </span>
              想看
            </p>
            <p>主演:{{ a.actor }}</p>
            <p>{{ a.showdate }}上映</p>
          </div>
        </div>
        <div class="w-1/6 py-4 h-full flex flex-col items-end">
          <p class="flex-1 text-orange-300">{{ a.scores }}分</p>
          <button class="rounded-xl w-12 h-8 text-sm bg-orange-400">
            预售
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
    img: "src/assets/images/20/01.jpg",
    title: "航海王：红发歌姬",
    wantsee: 613033,
    actor: "田中真弓,中井和哉,冈村明美",
    showdate: "2022-12-01",
    scores: 9.1,
  },
  {
    img: "src/assets/images/20/02.jpg",
    title: "放牛班的春天",
    wantsee: 613033,
    actor: "热拉尔·朱诺,弗朗西斯·贝尔兰德,凯德·麦拉德",
    showdate: "2022-12-01",
    scores: 9.1,
  },
  {
    img: "src/assets/images/20/03.jpg",
    title: "小小乔",
    wantsee: 613033,
    actor: "艾米丽·比查姆,本·威士肖,利安娜·贝斯特",
    showdate: "2022-12-01",
    scores: 9.1,
  },
  {
    img: "src/assets/images/20/04.jpg",
    title: "阿凡达：水之道",
    wantsee: 613033,
    actor: "萨姆·沃辛顿,佐伊·索尔达娜,西格妮·韦弗",
    showdate: "2022-12-01",
    scores: 9.1,
  },
]);
</script>

<style scoped></style>
