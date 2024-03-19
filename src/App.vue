<script setup>
import { onMounted, ref, watch } from 'vue'
import axios from 'axios'
import Header from './components/Header.vue'
import CardList from './components/CardList.vue'
import Drawer from './components/Drawer.vue'

const items = ref([])

const sortBy = ref('')
const searchQuery = ref('')

const onChangeSelect = (event) => {
 sortBy.value = event.target.value
}

onMounted(async () => {
  try {
    const { data } = await axios.get('https://0a55ea9c38d5267b.mokky.dev/items')
    items.value = data
  } catch (err) {
    console.log(err)
  }
})

watch(sortBy, async () => {
  try {
    const { data } = await axios.get(
      'https://0a55ea9c38d5267b.mokky.dev/items?sortBy=' + sortBy.value
    )
    items.value = data
  } catch (err) {
    console.log(err)
  }
})
</script>

<template>
  <!-- <Drawer/> -->
  <div class="bg-white w-4/5 m-auto rounded-xl shadow-xl mt-14">
    <Header />

    <div class="p-10">
      <div class="flex justify-between items-center">
        <h2 class="text-3xl font-bold mb-8">All Sneakers</h2>
        <div class="flex items-center gap-4">
          <select
            @change="onChangeSelect"
            class="py-2 px-3 border border-gray-200 focus:border-gray-400 rounded-md focus:outline-none"
          >
            <option value="name">By name</option>
            <option value="price">By price (cheap)</option>
            <option value="+price">By price (expensive)</option>
          </select>
          <div class="relative">
            <img class="absolute left-4 top-3" src="/search.svg" />
            <input
              class="border border-gray-200 rounded-md py-2 pl-10 pr-4 focus:outline-none focus:border-gray-400"
              placeholder="Search"
              type="text"
            />
          </div>
        </div>
      </div>

      <CardList :items="items" />
    </div>
  </div>
</template>
