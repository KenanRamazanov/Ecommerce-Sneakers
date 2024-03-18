<script setup>
import Card from './Card.vue'

defineProps({
  items: Array,
  isFavorites: Boolean
})

const onClickAdd = () => {
  alert('Elave olundu')
}
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
      v-for="item in items"
      :key="item.id"
      :id="item.id"
      :title="item.title"
      :imageUrl="item.imageUrl"
      :price="item.price"
      :onClickAdd="onClickAdd"
    />
  </div>
</template>
