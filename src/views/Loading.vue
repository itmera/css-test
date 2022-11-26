<template>
  <div class="flex flex-col h-screen items-center">
    <div class="flex gap-x-0.5 mt-10 animate-bounce">
      <p class="w-4 h-4 rounded-full bg-red-400"></p>
      <p class="w-4 h-4 rounded-full bg-blue-400"></p>
      <p class="w-4 h-4 rounded-full bg-yellow-400"></p>
    </div>

    <!-- 旋转➕减淡 -->
    <div class="grid grid-cols-2 w-16 h-16 gap-1 mt-20 animate-spin">
      <p class="w-4 h-4 rounded-full bg-red-400 animate-pulse"></p>
      <p class="w-4 h-4 rounded-full bg-blue-400"></p>
      <p class="w-4 h-4 rounded-full bg-yellow-400 animate-pulse"></p>
      <p class="w-4 h-4 rounded-full bg-purple-500"></p>
    </div>

    <!-- 旋转 -->
    <div class="mt-20 relative animate-spin">
      <div class="animate-pulse">
        <p class="absolute w-1 h-8 bg-green-400 -translate-y-10"></p>
        <p class="absolute w-1 h-8 bg-green-400 translate-y-2"></p>
        <p class="absolute w-8 h-1 bg-green-400 -translate-x-10"></p>
        <p class="absolute w-8 h-1 bg-green-400 translate-x-2"></p>
      </div>

      <div class="rotate-45 animate-pulse">
        <p class="absolute w-1 h-8 bg-green-400 -translate-y-10"></p>
        <p class="absolute w-1 h-8 bg-green-400 translate-y-2"></p>
        <p class="absolute w-8 h-1 bg-green-400 -translate-x-10"></p>
        <p class="absolute w-8 h-1 bg-green-400 translate-x-2"></p>
      </div>
    </div>

    <!-- 旋转的圆 -->
    <div class="mt-20 relative animate-spin">
      <p
        class="w-6 h-6 rounded-full border-2 border-red-500 border-t-transparent"
      ></p>
    </div>
  </div>
</template>

<style scoped>
@keyframes bounce {
  100% {
    transform: translateY(50%);
    animation-timing-function: cubic-bezier(0.8, 0, 1, 1);
  }
  0% {
    transform: translateY(-50%);
    animation-timing-function: cubic-bezier(0.8, 0, 1, 1);
  }
  50% {
    transform: none;
    animation-timing-function: cubic-bezier(0, 0, 0.6, 1);
  }
}
.animate-bounce {
  animation: bounce 2s 0.3s infinite;
}
.animate-bounce :nth-child(2) {
  animation: bounce 2s 0.5s infinite;
}
</style>
