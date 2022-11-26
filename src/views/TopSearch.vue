<template>
  <div>
    <div class="relative flex items-center space-x-2 pr-2 py-6">
      <div class="absolute left-3">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-5 h-5"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z"
          />
        </svg>
      </div>
      <input
        class="w-full h-10 border-2 rounded-md border-gray-300 flex-1 pl-6"
        type="text"
        placeholder="请输入搜索词"
      />
      <button class="bg-blue-400 rounded-lg w-16 h-9 text-white">搜索</button>
    </div>
  </div>
</template>

<style scoped></style>
