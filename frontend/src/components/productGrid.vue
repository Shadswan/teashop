<template>
  <div>
    <a>Сетка товаров</a>
  </div>
    <productCard 
      v-for="item in items"
        :name = "item.name"
        :img = "item.img"
        :decription = "item.decription"
    />
</template>

<script setup>
import productCard from './productCard.vue'

defineProps(['items'])

let items = [
  'name' = 'asd'
  'decription' = 'asddsdd'
]
</script>
