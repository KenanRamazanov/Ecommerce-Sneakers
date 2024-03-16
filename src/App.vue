<script setup>
import Header from './components/Header.vue'
import CardList from './components/CardList.vue'
import Drawer from './components/Drawer.vue'

const items = [
  
    {
        "id": 1,
        "title": "Men's Nike Blazer Mid Suede Sneakers",
        "price": 129.99,
        "imageUrl": "/sneakers/sneakers-1.jpg"
    },
    {
        "id": 2,
        "title": "Men's Nike Air Max 270 Sneakers",
        "price": 99.99,
        "imageUrl": "/sneakers/sneakers-2.jpg"
    },
    {
        "id": 3,
        "title": "Men's Nike Blazer Mid Suede Sneakers",
        "price": 88.99,
        "imageUrl": "/sneakers/sneakers-3.jpg"
    },
    {
        "id": 4,
        "title": "Puma X Sneakers, Aka Boku Future Rider",
        "price": 79.99,
        "imageUrl": "/sneakers/sneakers-4.jpg"
    },
    {
        "id": 5,
        "title": "Sneaker Future Rider",
        "price": 98.99,
        "imageUrl": "/sneakers/sneakers-5.jpg"
    },
    {
        "id": 6,
        "title": "Sneaker Black Edition",
        "price": 145.99,
        "imageUrl": "/sneakers/sneakers-6.jpg"
    },
    {
        "id": 7,
        "title": "Sneaker Orange Boomb Edition",
        "price": 126.99,
        "imageUrl": "/sneakers/sneakers-7.jpg"
    },
    {
        "id": 8,
        "title": "Sneaker Nike Air Max 270",
        "price": 156.99,
        "imageUrl": "/sneakers/sneakers-8.jpg"
    },
    {
        "id": 9,
        "title": "Sneaker Nike Air Force 1",
        "price": 59,
        "imageUrl": "/sneakers/sneakers-9.jpg"
    },
    {
        "id": 10,
        "title": "Sneaker Adidas Ultraboost",
        "price": 115.99,
        "imageUrl": "/sneakers/sneakers-10.jpg"
    },
    {
        "id": 11,
        "title": "Sneaker Puma Clyde All-Pro",
        "price": 76.99,
        "imageUrl": "/sneakers/sneakers-11.jpg"
    },
    {
        "id": 12,
        "title": "Sneaker Converse Chuck Taylor All-Star",
        "price": 129.99,
        "imageUrl": "/sneakers/sneakers-12.jpg"
    },
    {
        "name": "Root",
        "email": "admin@email.com",
        "id": 13
    },
    {
        "id": 14
    },
    {
        "0": {
            "id": 1,
            "title": "Men's Nike Blazer Mid Suede Sneakers",
            "price": 129.99,
            "imageUrl": "/sneakers/sneakers-1.jpg",
            "isFavorite": true,
            "favoriteId": 3,
            "isAdded": false
        },
        "1": {
            "id": 2,
            "title": "Men's Nike Air Max 270 Sneakers",
            "price": 99.99,
            "imageUrl": "/sneakers/sneakers-2.jpg",
            "isFavorite": true,
            "favoriteId": 1,
            "isAdded": false
        },
        "2": {
            "id": 3,
            "title": "Men's Nike Blazer Mid Suede Sneakers",
            "price": 88.99,
            "imageUrl": "/sneakers/sneakers-3.jpg",
            "isFavorite": true,
            "favoriteId": 2,
            "isAdded": false
        },
        "3": {
            "id": 4,
            "title": "Puma X Sneakers, Aka Boku Future Rider",
            "price": 79.99,
            "imageUrl": "/sneakers/sneakers-4.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "4": {
            "id": 5,
            "title": "Sneaker Future Rider",
            "price": 98.99,
            "imageUrl": "/sneakers/sneakers-5.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "5": {
            "id": 6,
            "title": "Sneaker Black Edition",
            "price": 145.99,
            "imageUrl": "/sneakers/sneakers-6.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "6": {
            "id": 7,
            "title": "Sneaker Orange Boomb Edition",
            "price": 126.99,
            "imageUrl": "/sneakers/sneakers-7.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "7": {
            "id": 8,
            "title": "Sneaker Nike Air Max 270",
            "price": 156.99,
            "imageUrl": "/sneakers/sneakers-8.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "8": {
            "id": 9,
            "title": "Sneaker Nike Air Force 1",
            "price": 59,
            "imageUrl": "/sneakers/sneakers-9.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "9": {
            "id": 10,
            "title": "Sneaker Adidas Ultraboost",
            "price": 115.99,
            "imageUrl": "/sneakers/sneakers-10.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "10": {
            "id": 11,
            "title": "Кроссовки Puma Clyde All-Pro",
            "price": 7600,
            "imageUrl": "/sneakers/sneakers-11.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "11": {
            "id": 12,
            "title": "Sneaker Converse Chuck Taylor All-Star",
            "price": 129.99,
            "imageUrl": "/sneakers/sneakers-12.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "12": {
            "name": "Root",
            "email": "admin@email.com",
            "id": 13,
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "13": {
            "id": 14,
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "id": 15
    },
    {
        "0": {
            "title": "Men's Nike Blazer Mid Suede Sneakers",
            "price": 129.99,
            "imageUrl": "/sneakers/sneakers-1.jpg",
            "isFavorite": true,
            "favoriteId": 3,
            "isAdded": false
        },
        "1": {
            "id": 2,
            "title": "Men's Nike Air Max 270 Sneakers",
            "price": 99.99,
            "imageUrl": "/sneakers/sneakers-2.jpg",
            "isFavorite": true,
            "favoriteId": 1,
            "isAdded": false
        },
        "2": {
            "id": 3,
            "title": "Men's Nike Blazer Mid Suede Sneakers",
            "price": 88.99,
            "imageUrl": "/sneakers/sneakers-3.jpg",
            "isFavorite": true,
            "favoriteId": 2,
            "isAdded": false
        },
        "3": {
            "id": 4,
            "title": "Puma X Sneakers, Aka Boku Future Rider",
            "price": 79.99,
            "imageUrl": "/sneakers/sneakers-4.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "4": {
            "id": 5,
            "title": "Sneaker Future Rider",
            "price": 98.99,
            "imageUrl": "/sneakers/sneakers-5.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "5": {
            "id": 6,
            "title": "Sneaker Black Edition",
            "price": 145.99,
            "imageUrl": "/sneakers/sneakers-6.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "6": {
            "id": 7,
            "title": "Sneaker Orange Boomb Edition",
            "price": 126.99,
            "imageUrl": "/sneakers/sneakers-7.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "7": {
            "id": 8,
            "title": "Sneaker Nike Air Max 270",
            "price": 156.99,
            "imageUrl": "/sneakers/sneakers-8.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "8": {
            "id": 9,
            "title": "Sneaker Nike Air Force 1",
            "price": 59,
            "imageUrl": "/sneakers/sneakers-9.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "9": {
            "id": 10,
            "title": "Sneaker Adidas Ultraboost",
            "price": 115.99,
            "imageUrl": "/sneakers/sneakers-10.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "10": {
            "id": 11,
            "title": "Sneaker Puma Clyde All-Pro",
            "price": 76.99,
            "imageUrl": "/sneakers/sneakers-11.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "11": {
            "id": 12,
            "title": "Sneaker Converse Chuck Taylor All-Star",
            "price": 129.99,
            "imageUrl": "/sneakers/sneakers-12.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "id": 16
    },
    {
        "0": {
            "title": "Men's Nike Blazer Mid Suede Sneakers",
            "price": 129.99,
            "imageUrl": "/sneakers/sneakers-1.jpg",
            "isFavorite": true,
            "favoriteId": 3,
            "isAdded": false
        },
        "1": {
            "id": 2,
            "title": "Men's Nike Air Max 270 Sneakers",
            "price": 99.99,
            "imageUrl": "/sneakers/sneakers-2.jpg",
            "isFavorite": true,
            "favoriteId": 1,
            "isAdded": false
        },
        "2": {
            "id": 3,
            "title": "Men's Nike Air Max 270 Sneakers",
            "price": 99.99,
            "imageUrl": "/sneakers/sneakers-3.jpg",
            "isFavorite": true,
            "favoriteId": 2,
            "isAdded": false
        },
        "3": {
            "id": 4,
            "title": "Puma X Sneakers, Aka Boku Future Rider",
            "price": 79.99,
            "imageUrl": "/sneakers/sneakers-4.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "4": {
            "id": 5,
            "title": "Sneaker Future Rider",
            "price": 98.99,
            "imageUrl": "/sneakers/sneakers-5.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "5": {
            "id": 6,
            "title": "Sneaker Black Edition",
            "price": 145.99,
            "imageUrl": "/sneakers/sneakers-6.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "6": {
            "id": 7,
            "title": "Sneaker Orange Boomb Edition",
            "price": 126.99,
            "imageUrl": "/sneakers/sneakers-7.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "7": {
            "id": 8,
            "title": "Sneaker Nike Air Max 270",
            "price": 156.99,
            "imageUrl": "/sneakers/sneakers-8.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "8": {
            "id": 9,
            "title": "Sneaker Nike Air Force 1",
            "price": 59,
            "imageUrl": "/sneakers/sneakers-9.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "9": {
            "id": 10,
            "title": "Sneaker Adidas Ultraboost",
            "price": 115.99,
            "imageUrl": "/sneakers/sneakers-10.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "10": {
            "id": 11,
            "title": "Sneaker Puma Clyde All-Pro",
            "price": 76.99,
            "imageUrl": "/sneakers/sneakers-11.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "11": {
            "id": 12,
            "title": "Sneaker Converse Chuck Taylor All-Star",
            "price": 129.99,
            "imageUrl": "/sneakers/sneakers-12.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "id": 17
    },
    {
        "0": {
            "id": 1,
            "title": "Men's Nike Blazer Mid Suede Sneakers",
            "price": 129.99,
            "imageUrl": "/sneakers/sneakers-1.jpg",
            "isFavorite": true,
            "favoriteId": 3,
            "isAdded": false
        },
        "1": {
            "id": 2,
            "title": "Men's Nike Air Max 270 Sneakers",
            "price": 99.99,
            "imageUrl": "/sneakers/sneakers-2.jpg",
            "isFavorite": true,
            "favoriteId": 1,
            "isAdded": false
        },
        "2": {
            "id": 3,
            "title": "Men's Nike Blazer Mid Suede Sneakers",
            "price": 88.99,
            "imageUrl": "/sneakers/sneakers-3.jpg",
            "isFavorite": true,
            "favoriteId": 2,
            "isAdded": false
        },
        "3": {
            "id": 4,
            "title": "Puma X Sneakers, Aka Boku Future Rider",
            "price": 79.99,
            "imageUrl": "/sneakers/sneakers-4.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "4": {
            "id": 5,
            "title": "Sneaker Future Rider",
            "price": 98.99,
            "imageUrl": "/sneakers/sneakers-5.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "5": {
            "id": 6,
            "title": "Sneaker Black Edition",
            "price": 145.99,
            "imageUrl": "/sneakers/sneakers-6.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "6": {
            "id": 7,
            "title": "Sneaker Orange Boomb Edition",
            "price": 126.99,
            "imageUrl": "/sneakers/sneakers-7.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "7": {
            "id": 8,
            "title": "Sneaker Nike Air Max 270",
            "price": 156.99,
            "imageUrl": "/sneakers/sneakers-8.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "8": {
            "id": 9,
            "title": "Sneaker Nike Air Force 1",
            "price": 59,
            "imageUrl": "/sneakers/sneakers-9.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "9": {
            "id": 10,
            "title": "Sneaker Adidas Ultraboost",
            "price": 115.99,
            "imageUrl": "/sneakers/sneakers-10.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "10": {
            "id": 11,
            "title": "Sneaker Puma Clyde All-Pro",
            "price": 76.99,
            "imageUrl": "/sneakers/sneakers-11.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "11": {
            "id": 12,
            "title": "Sneaker Converse Chuck Taylor All-Star",
            "price": 129.99,
            "imageUrl": "/sneakers/sneakers-12.jpg",
            "isFavorite": false,
            "favoriteId": null,
            "isAdded": false
        },
        "id": 18
    },
    {
        "id": 19
    }
]


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
            class="py-2 px-3 border border-gray-200 focus:border-gray-400 rounded-md focus:outline-none"
          >
            <option value="name">By name</option>
            <option value="price">By price (cheap)</option>
            <option value="price">By price (expensive)</option>
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
