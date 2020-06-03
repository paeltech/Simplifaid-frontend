<template>
  <div class="wrapper">
    <header class="top-bar py-8 rounded-lg">
      <div class="float-left">
        <h1 class="text-4xl tracking-wider">
          Hello,
          <span class="font-bold capitalize">{{ user.name }}</span>
        </h1>
      </div>
      <div class="float-right">
        <a href="#">
          <ion-icon name="person-outline"></ion-icon>Account
        </a>
      </div>
    </header>
    <div class="clearfix wid-100"></div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.wid-100 {
  width: 100%;
  overflow: hidden;
}
</style>