<template>
  <div class="bg-gray-300 h-screen">
    <div class="h-3"></div>

    <div class="bg-white m-3 rounded-xl">
      <div class="flex justify-between">
        <div class="w-1/3 m-2">
          <img
            src="src/assets/images/18/02.webp"
            class="w-full h-full rounded-lg"
            alt=""
          />
        </div>
        <div class="flex-1 flex flex-col">
          <p class="h-1/3 pt-3 overflow-hidden text-lg leading-6">
            AMAKUNI 超次元游戏海王星 縔色之心 手办
          </p>
          <div class="flex-1 flex justify-between">
            <div class="flex-1 flex justify-evenly gap-1 self-end my-2">
              <div class="w-1/3">
                <img
                  src="src/assets/images/18/02.webp"
                  class="rounded-sm"
                  alt=""
                />
              </div>
              <div class="w-1/3">
                <img
                  src="src/assets/images/18/03.webp"
                  class="rounded-sm"
                  alt=""
                />
              </div>
              <div class="w-1/3">
                <img
                  src="src/assets/images/18/04.webp"
                  class="rounded-sm"
                  alt=""
                />
              </div>
            </div>
            <button
              class="self-end mx-2 mb-2 px-2 text-pink-300 border border-pink-300 rounded-xl"
            >
              订阅
            </button>
          </div>
        </div>
      </div>
      <!-- 点赞 订阅 -->
      <div class="flex justify-between p-2 text-gray-400 text-sm">
        <div class="flex space-x-1">
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
              d="M12 20.25c4.97 0 9-3.694 9-8.25s-4.03-8.25-9-8.25S3 7.444 3 12c0 2.104.859 4.023 2.273 5.48.432.447.74 1.04.586 1.641a4.483 4.483 0 01-.923 1.785A5.969 5.969 0 006 21c1.282 0 2.47-.402 3.445-1.087.81.22 1.668.337 2.555.337z"
            />
          </svg>
          <p>{{ Math.floor(Math.random() * 100) }}</p>
        </div>
        <p>{{ Math.floor(Math.random() * 9000) + 1000 }}人已订阅</p>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
