<script setup>
import { inject } from 'vue';
import Card from './Card.vue'

defineProps({
  items: Array,
  isFavorites: Boolean,
  addToFavorite: Function,
})

const onClickAdd = () => {
  alert('Elave olundu')
}

const addToFavorite = inject('addToFavorite')

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
      :onClickFavorite="() => addToFavorite(item)"
      :isFavorite="item.isFavorite"
    />
  </div>
</template>
