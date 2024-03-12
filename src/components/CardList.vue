<script setup>
import Card from "./Card.vue";


const onClickAdd = () => {
    alert("Elave olundu")
}
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card 
    title="Men's Nike Blazer Mid Suede"
     imageUrl="/sneakers/sneakers-1.jpg" 
     :price="142.99"
    :isAdded="true"
     :isFavorite="true"
     :onClickAdd="onClickAdd"
     />
 
  </div>
</template>
