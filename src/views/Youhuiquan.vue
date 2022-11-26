<template>
  <div class="bg-gray-700 w-full h-screen relative">
    <!-- 优惠券 -->
    <div class="absolute inset-x-0 h-[80%] bottom-0 top-15 bg-white">
      <h2 class="text-center text-2xl p-3">优惠</h2>
      <div class="space-y-2 text-gray-600 px-2">
        <h3 class="text-gray-400">促销</h3>
        <p>
          <span class="text-red-400 px-2">限购</span>
          <span>每人限购5件;此优惠限量5件,超出则该商品全部恢复非活动价</span>
        </p>
        <p>
          <span class="text-red-400 px-2">积分</span><span>购买可得59积分</span>
        </p>
      </div>
      <div class="flex items-center justify-between py-4 px-2 text-gray-400">
        <h3>领券</h3>
        <p>已有积分：3999</p>
      </div>
      <div class="grid text-red-400 gap-2 px-1">
        <div
          class="flex self-center items-center text-xs"
          v-for="(a, i) in 40"
          :key="i"
        >
          <div class="flex-1 p-1 h-20 rounded-lg rounded-r-2xl bg-red-100">
            <p>
              <span class="text-2xl pr-2"
                >￥{{ Math.floor(a * Math.random() * 20) }}</span
              >店铺优惠券
            </p>
            <p>满{{ (a * 99) / 2 }}可用</p>
            <p>有效期：2022年11月1日--2023年1月1日</p>
          </div>
          <p
            class="h-20 py-5 text-base leading-10 px-4 rounded-r-lg bg-red-100 rounded-l-2xl"
          >
            立即领取
          </p>
        </div>
      </div>
      <div class="h-12"></div>
      <!-- 按钮 -->
      <button
        class="w-full h-10 text-xl text-white leading-10 bg-red-500 fixed left-0 bottom-0"
      >
        完成
      </button>
    </div>
  </div>
</template>

<style scoped></style>
