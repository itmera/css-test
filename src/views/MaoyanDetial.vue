<template>
  <div class="bg-gray-200 h-screen relative">
    <img src="src/assets/images/20/01.jpg" alt="" class="w-full h-72 blur-xl" />
    <div class="gap-2 absolute inset-0">
      <div class="px-2 h-48 flex justify-between items-center">
        <div class="w-1/4 relative px-1">
          <img src="src/assets/images/20/01.jpg" class="rounded-xl" alt="" />
          <div class="absolute inset-0 flex justify-center items-center">
            <p class="text-xl text-white">▶️</p>
          </div>
        </div>
        <div class="flex-1 flex flex-col px-2 justify-between">
          <p class="text-lg">
            航海王：红发歌姬
            <span class="bg-blue-300 border text-white rounded-l text-xs"
              >3D</span
            >
            <span class="text-blue-300 border border-blue-300 rounded-r text-xs"
              >MAX</span
            >
          </p>
          <div class="text-gray-400">
            <p>One Piece Film Red</p>
            <p>动画</p>

            <p>主演:田中真弓 中井和哉 冈村明美</p>
            <p>2022-12-01上映 <span>中国大陆上映/115分钟</span></p>
          </div>
        </div>
      </div>
      <div class="flex justify-evenly p-2 gap-2 text-white">
        <button class="w-1/2 bg-white/40 rounded h-10">想看</button>
        <button class="w-1/2 bg-white/40 rounded h-10">评分</button>
      </div>
      <!-- b -->
      <p class="bg-white p-2 text-gray-500">
        令全世界为之疯狂的歌姬·乌塔，她的身世成谜，歌声却被誉为“来自别的次元”。而这次，她将举办演唱会并第一次露出庐山真面目。为了欣赏她的歌声，路飞率领的草帽一伙，以及世界各地的歌迷都汇聚在会场之中。全世界备受瞩目的歌声即将在此回荡。而故事就在乌塔是“杰克斯的女儿”这一令人震惊的发现中拉开帷幕！
      </p>
      <div class="bg-white my-2">
        <p class="p-2">演职人员</p>
        <div class="grid grid-cols-4 gap-2 p-4">
          <img src="src/assets/images/21/112.jpeg" alt="" class="rounded-xl" />
          <img src="src/assets/images/21/113.jpg" alt="" class="rounded-xl" />
          <img src="src/assets/images/21/114.jpg" alt="" class="rounded-xl" />
          <img src="src/assets/images/21/115.jpg" alt="" class="rounded-xl" />
        </div>
      </div>
      <div class="bg-white">
        <p class="p-2">票房</p>
        <div
          class="grid grid-cols-3 gap-2 p-4 items-center justify-items-center"
        >
          <div class="flex flex-col items-center">
            <p class="text-3xl text-red-600">7</p>
            <p>昨日票房排行</p>
          </div>
          <div class="flex flex-col items-center">
            <p class="text-xl text-gray-400">暂无</p>
            <p>首周票房(万)</p>
          </div>
          <div class="flex flex-col items-center">
            <p class="text-3xl text-red-600">3971</p>
            <p>累计票房(万)</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
