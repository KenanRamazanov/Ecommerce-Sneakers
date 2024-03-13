<script setup>
import Header from './components/Header.vue'
import CardList from './components/CardList.vue'
import Drawer from './components/Drawer.vue'


</script>

<template>
 <!-- <Drawer/> -->
  <div class="bg-white w-4/5 m-auto rounded-xl shadow-xl mt-14">
    <Header />

    <div class="p-10">
     <div class="flex justify-between">
      <h2 class="text-3xl font-bold mb-8">All Sneakers</h2>
        <div>
           <input 
           placeholder="Search"
           type="text">
        </div>
     </div>

     <CardList/>
    </div>
  </div>
</template>
