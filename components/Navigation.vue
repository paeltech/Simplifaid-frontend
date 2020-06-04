<template>
  <nav class="flex flex-row md:justify-between">
    <div class="flex flex-row justify-between">
      <div>
        <nuxt-link to="/">
          <img class="w-8 md:w-10" src="~/static/img/logo.png" alt />
        </nuxt-link>
      </div>
      <div class="md:hidden absolute right-0 mt-2 mr-2 hamburger" @click="isOpen = !isOpen">
        <ion-icon name="menu-outline"></ion-icon>
      </div>
    </div>
    <ul :class="isOpen ? 'block' : 'hidden'" class="md:flex md:flex-row mt-8 md:mt-2">
      <!-- <li class="mr-6 mt-4">
        <nuxt-link to="/login">
          <ion-icon name="person-circle-outline"></ion-icon>Account
        </nuxt-link>
      </li>-->
      <li class="mr-6 mt-4">
        <a href="#" class="hover:text-green-600">
          <ion-icon name="help-circle-outline"></ion-icon>Help
        </a>
      </li>
      <li class="mr-6 mt-4">
        <a href="#" class="hover:text-green-600">
          <ion-icon name="cart-outline"></ion-icon>Basket
          <span
            class="flex content-center justify-center w-6 h-6 ml-2 rounded-full bg-black text-white float-right"
          >3</span>
        </a>
      </li>
      <li v-if="!authenticated" class="mt-4">
        <nuxt-link class="bg-green-600 text-white rounded px-4 py-2" to="/login">Login</nuxt-link>
      </li>
      <li v-if="authenticated" class="mt-4 capitalize">
        {{user.name}}
        <a
          href
          @click.prevent="logout"
          class="bg-green-600 text-white rounded px-4 py-2"
        >Logout</a>
      </li>
    </ul>
  </nav>
</template>

<style scoped>
ion-icon {
  font-size: 18px;
  vertical-align: middle;
  padding-bottom: 3px;
  padding-right: 10px;
}

.hamburger ion-icon {
  font-size: 26px;
}
</style>

<script>
export default {
  data() {
    return {
      isOpen: false
    }
  },
  methods: {
    logout() {
      this.$auth.logout()
    }
  }
}
</script>
