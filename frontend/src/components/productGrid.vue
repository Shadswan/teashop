<template>
  <div>
    <a>Сетка товаров</a>
  </div>
  <div v-for="item in items">
    {{item}}
  </div>
</template>

<script setup>
let items = [1,2,3,4]
</script>
