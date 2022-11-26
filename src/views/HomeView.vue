<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <div class="min-w-full bg-green-200 min-h-screen">
    8888
    <ul>
      <li><router-link :to="{ name: 'home' }">home</router-link></li>
      <li><router-link :to="{ name: 'me' }">me</router-link></li>
    </ul>
  </div>
</template>
