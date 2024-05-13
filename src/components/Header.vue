<script setup>
defineProps({
  totalPrice: Number
})

const emit = defineEmits(['openDrawer'])
</script>


<template>
  <header class="flex justify-between border-b border-slate-200 px-10 py-8">
    <router-link to="/">
    <div class="flex items-center gap-4">
      <img src="/logo.png" alt="Logo" class="w-11" />
      <div>
        <h2 class="font-bold text-xl uppercase">Vue Sneakers</h2>
        <p class="text-slate-400">Shop for the best sneakers</p>
      </div>
    </div>
  </router-link>

    <ul class="flex items-center gap-10">
      <li
      @click="() => emit('openDrawer')"
      class="flex items-center gap-3 cursor-pointer text-gray-500 hover:text-black">
        <img src="/cart.svg" alt="Cart" />
        <b> {{totalPrice}} руб</b>
      </li>
      <router-link to="/favorites">
        <li class="flex items-center gap-3 cursor-pointer text-gray-500 hover:text-black">
          <img src="/heart.svg" alt="Favorite" />
          <span>Favorites</span>
        </li>

      </router-link>
      <li class="flex items-center gap-3 cursor-pointer text-gray-500 hover:text-black">
        <img src="/profile.svg" alt="Favorite" />
        <span>Profile</span>
      </li>
    </ul>
  </header>
</template>
