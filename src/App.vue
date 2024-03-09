<template>
  <div class="bg-white w-4/5 m-auto h-screen rounded-xl shadow-xl mt-14">
    <header class="flex justify-between border-b border-slate-200 px-10 py-8">
      <div class="flex items-center gap-4">
        <img src="/logo.png" alt="Logo" class="w-11" />
        <div>
          <h2 class="font-bold text-xl uppercase">Vue Sneakers</h2>
          <p class="text-slate-400">Shop for the best sneakers</p>
        </div>
      </div>

      <ul class="flex items-center gap-10">
        <li class="flex items-center gap-3 cursor-pointer  text-gray-500  hover:text-black">
          <img src="/cart.svg" alt="Cart" />
          <b>1205 usd</b>
        </li>
        <li class="flex items-center gap-3 cursor-pointer text-gray-500  hover:text-black">
          <img src="/heart.svg" alt="Favorite" />
          <span>Favorites</span>
        </li>
        <li class="flex items-center gap-3 cursor-pointer text-gray-500 hover:text-black">
          <img src="/profile.svg" alt="Favorite" />
          <span>Profile</span>
        </li>
      </ul>
    </header>

    <h1>Ramazanov Blog</h1>
  </div>
</template>
