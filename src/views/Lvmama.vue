<template>
  <div class="bg-gray-100 h-screen relative">
    <!-- 头部图片 -->
    <div class="w-full">
      <img src="src/assets/images/19/th.jpeg" class="w-full h-64" alt="" />
    </div>
    <!-- 中国上海 -->
    <div class="absolute top-10 inset-x-5 flex flex-col">
      <div class="flex text-gray-200">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 24"
          fill="currentColor"
          class="w-6 h-6"
        >
          <path
            fill-rule="evenodd"
            d="M11.54 22.351l.07.04.028.016a.76.76 0 00.723 0l.028-.015.071-.041a16.975 16.975 0 001.144-.742 19.58 19.58 0 002.683-2.282c1.944-1.99 3.963-4.98 3.963-8.827a8.25 8.25 0 00-16.5 0c0 3.846 2.02 6.837 3.963 8.827a19.58 19.58 0 002.682 2.282 16.975 16.975 0 001.145.742zM12 13.5a3 3 0 100-6 3 3 0 000 6z"
            clip-rule="evenodd"
          />
        </svg>

        <p>中国</p>
      </div>
      <div class="flex text-white my-2">
        <p class="h-10 leading-10 text-2xl px-1">上海</p>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 24"
          fill="currentColor"
          class="w-6 h-6 self-center"
        >
          <path
            fill-rule="evenodd"
            d="M12 2.25c-5.385 0-9.75 4.365-9.75 9.75s4.365 9.75 9.75 9.75 9.75-4.365 9.75-9.75S17.385 2.25 12 2.25zm-.53 14.03a.75.75 0 001.06 0l3-3a.75.75 0 10-1.06-1.06l-1.72 1.72V8.25a.75.75 0 00-1.5 0v5.69l-1.72-1.72a.75.75 0 00-1.06 1.06l3 3z"
            clip-rule="evenodd"
          />
        </svg>
      </div>
      <div class="self-end relative text-gray-500">
        <input
          class="h-8 w-40 pl-8 text-lg rounded-full bg-white/75"
          type="text"
          placeholder="目的地/游记"
          name=""
          id=""
        />
        <div class="absolute top-0 left-2 py-1 text-gray-400">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            fill="currentColor"
            class="w-6 h-6"
          >
            <path
              fill-rule="evenodd"
              d="M10.5 3.75a6.75 6.75 0 100 13.5 6.75 6.75 0 000-13.5zM2.25 10.5a8.25 8.25 0 1114.59 5.28l4.69 4.69a.75.75 0 11-1.06 1.06l-4.69-4.69A8.25 8.25 0 012.25 10.5z"
              clip-rule="evenodd"
            />
          </svg>
        </div>
      </div>
      <div class="bg-white mt-8 rounded-2xl grid grid-cols-5 py-6">
        <div class="flex flex-col items-center">
          <img
            src="src/assets/images/19/bangdan.png"
            alt=""
            class="w-3/5 rounded-lg"
          />

          <p>榜单</p>
        </div>
        <div class="flex flex-col items-center">
          <img
            src="src/assets/images/19/meishi.png"
            alt=""
            class="w-3/5 rounded-lg"
          />
          <p>美食</p>
        </div>
        <div class="flex flex-col items-center">
          <img
            src="src/assets/images/19/gouwu.png"
            alt=""
            class="w-3/5 rounded-lg"
          />
          <p>购物</p>
        </div>
        <div class="flex flex-col items-center">
          <img
            src="src/assets/images/19/yule.png"
            alt=""
            class="w-3/5 rounded-lg"
          />
          <p>娱乐</p>
        </div>
        <div class="flex flex-col items-center">
          <img
            src="src/assets/images/19/xingcheng.png"
            alt=""
            class="w-3/5 rounded-lg"
          />
          <p>行程</p>
        </div>
      </div>

      <!-- 旅游指南 -->
      <div class="bg-blue-100 mt-4 rounded-lg">
        <div class="flex justify-between">
          <div class="flex gap-1 p-2">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="currentColor"
              class="w-6 h-6 text-blue-400"
            >
              <path
                d="M3.478 2.405a.75.75 0 00-.926.94l2.432 7.905H13.5a.75.75 0 010 1.5H4.984l-2.432 7.905a.75.75 0 00.926.94 60.519 60.519 0 0018.445-8.986.75.75 0 000-1.218A60.517 60.517 0 003.478 2.405z"
              />
            </svg>

            <p class="h-6 text-lg leading-6">旅游指南</p>
          </div>
          <p class="p-2 text-sm text-gray-500">更多》</p>
        </div>
        <p class="text-sm text-gray-400 p-2">
          十里洋场万国建筑，浦江两岸华灯璀璨，弄堂里面的新天地，梧桐树下的老洋房，千面之城，魅力魔都。
        </p>
        <div class="flex justify-between text-blue-400 text-center p-4">
          <p class="w-1/3 px-4 rounded-full bg-white">初始印象</p>
          <p class="w-1/3 px-4 rounded-full bg-white">行前必知</p>
          <p class="w-1/3 px-4 rounded-full bg-white">必游TOP</p>
        </div>
      </div>
      <!-- 精选榜单 -->
      <div class="bg-white mt-4 rounded-lg">
        <div class="flex justify-between">
          <p class="h-6 text-lg leading-6 p-2">精选榜单</p>

          <p class="p-2 text-sm text-gray-500">更多》</p>
        </div>

        <div class="flex justify-between text-white text-center gap-2 p-2">
          <p class="w-1/3 p-3 rounded bg-pink-300">全球地标建 筑巡礼</p>
          <p class="w-1/3 p-3 rounded bg-purple-400">独自旅行•境内篇</p>
          <p class="w-1/3 p-3 rounded bg-blue-300">打卡江浙沪 露营地</p>
        </div>
      </div>
      <!-- 热门城市 -->
      <div class="bg-white mt-4 rounded-lg">
        <div class="flex justify-between">
          <p class="h-6 text-lg leading-6 p-2">热门城市</p>

          <p class="p-2 text-sm text-gray-500">更多》</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
