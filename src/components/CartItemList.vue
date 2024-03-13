<script setup>
import CartItem from './CartItem.vue';


const onClickAdd = () => {
    alert("Elave olundu")
}
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <CartItem 
    title="Men's Nike Blazer Mid Suede"
     imageUrl="/sneakers/sneakers-1.jpg" 
     :price="142.99"
    :isAdded="true"
     :isFavorite="true"
     :onClickAdd="onClickAdd"
     />
 
  </div>
</template>
