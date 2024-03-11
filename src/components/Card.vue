<script setup>
defineProps({
  imageUrl: String,
  title: String,
  price: Number,
  isFavorite: Boolean,
  isAdded: Boolean
})
</script>

<template>
  <div
    class="relative border bg-white border-slate-100 rounded-3xl p-8 cursor-pointer hover:-translate-y-2 hover:shadow-xl transition"
  >
    <img src="/like-2.svg" alt="Like 2" class="absolute top-8 left-8" />
    <img :src="imageUrl" alt="Sneakers" />
    <p class="mt-2">{{ title }}</p>

    <div class="flex justify-between mt-5">
      <div class="flex flex-col gap-2">
        <span class="text-slate-400">Price:</span>
        <span class="font-bold">{{ price }}</span>
      </div>

      <img :src="!isAdded ? '/plus.svg' : '/checked.svg' " alt="Plus" />
    </div>
  </div>
</template>
