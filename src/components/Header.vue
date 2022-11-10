<script setup>
import { ref } from 'vue';

defineProps({
  // msg: String
});

const count = ref(0);
</script>

<template>
  <div class="headerBox">
    <ul class="heaUl">
      <li>首页</li>
      <li>Code</li>
      <li>关于</li>
    </ul>
  </div>
</template>

<style scoped>
.heaUl {
  width: 100%;
  height: 200px;
  border: 2px solid #000;
}
.heaUl li {
  list-style: none;
}
</style>
