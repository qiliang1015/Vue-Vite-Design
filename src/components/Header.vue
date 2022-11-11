<script setup>
import { ref } from 'vue';

defineProps({
  // msg: String
});

const count = ref(0);
</script>

<template>
  <div class="headerBox">
    <div class="helLeftLogoTitle"></div>
    <ul class="heaUl">
      <li>
        <a href="#">Home</a>
      </li>
      <li>
        <a href="#">Code</a>
      </li>
      <li>
        <a href="#">About</a>
      </li>
    </ul>
    <div class="heaRightTools"></div>
  </div>
</template>

<style scoped>
.headerBox {
  display: flex;
  height: 60px;
  justify-content: space-between;
  background-color: #141f29;
  box-shadow: 0 -10px 60px -12px;
  --tw-shadow-color: rgba(99, 102, 241, 0.4);
}
.helLeftLogoTitle {
  flex: 0.3;
}
.heaUl {
  width: 600px;
  display: flex;
  justify-content: space-around;
  border-left: 1px solid #000;
  border-right: 1px solid #000;
}
.heaUl li {
  list-style: none;
  display: flex;
  align-items: center;
}
.heaUl li a {
  color: #fff;
  width: 60px;
  border-bottom: 1px solid #fff;
  border-top: 1px solid #fff;
  text-align: center;
  text-decoration: none;
  padding: 5px;
}
.heaUl li a:hover {
  transition:.5s;
  color: #2fc0c9;
  border-color: #2fc0c9;
}

.heaRightTools {
  flex: 0.2;
}
</style>
