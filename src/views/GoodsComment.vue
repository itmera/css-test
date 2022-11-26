<template>
  <div class="flex flex-wrap text-sm">
    <p
      v-for="(a, i) in commentList"
      :key="i"
      class="bg-orange-200 rounded-xl px-2 py-0.5 m-1"
    >
      {{ a.text }} <span class="text-xs">({{ a.num }})</span>
    </p>
  </div>
</template>

<script setup>
import { ref } from "vue";

const commentList = ref([
  { text: "汤色纯正方便实用", num: 16 },
  { text: "茶香四溢", num: 6 },
  { text: "分量充足", num: 5 },
  { text: "颗粒硕大", num: 3 },
  { text: "色泽通透", num: 3 },
  { text: "风味十足", num: 3 },
  { text: "做工精良", num: 2 },
  { text: "清香软糯", num: 1 },
  { text: "味道浓厚", num: 1 },
  { text: "香糯可口", num: 7 },
  { text: "营养丰富", num: 42 },
]);
</script>

<style scoped></style>
