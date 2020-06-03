<template>
  <div class="wrapper">
    <h1 class="text-xl font-bold text-white">
      Simplifaid
      <span class="float-right menu">
        <ion-icon name="menu-outline"></ion-icon>
      </span>
    </h1>
    <div class="pt-4"></div>
    <ul class="text-gray-400">
      <li>
        <a href="#">Dashboard</a>
      </li>
      <li>
        <a href="#">Users</a>
      </li>
      <li>
        <nuxt-link to="/profile/products">Products</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/profile/vendors">Vendors</nuxt-link>
      </li>
      <li>
        <a href="#">Orders</a>
      </li>
      <li>
        <a href="#">Settings</a>
      </li>
      <li class="mt-4">
        <nuxt-link to="/logout">Logout</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<style scoped>
.wrapper {
  height: 100vh;
}
</style>