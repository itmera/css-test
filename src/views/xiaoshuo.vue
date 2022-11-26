<template>
  <div>
    <div class="mt-10 pl-3 text-2xl">达人们的戏精小剧场</div>

    <div class="grid grid-cols-2 gap-2 mt-3 p-2">
      <div class="relative" v-for="a in 8" :key="a">
        <div class="absolute inset-0 top-8 bg-gray-100 rounded-xl -z-10"></div>
        <div class="flex flex-col px-2 py-4">
          <img
            :src="`src/assets/images/22/30${a + 1}.jpg`"
            alt=""
            class="w-24 h-24 rounded-lg"
          />
          <p class="h-10 text-lg leading-10">王者峡谷搞笑时刻{{ a }}</p>
          <p class="h-16 text-gray-500">青铜操作有没有秀到你，订阅我收获快乐</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
