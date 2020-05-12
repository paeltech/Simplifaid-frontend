<template>
  <div class="prod-header-bg">
    <div class="container mx-auto p-6">
      <Navigation />
      <div class="w-5/6 mx-auto mt-16 text-center">
        <div class="inline-block relative">
          <select
            name="categories"
            id=""
            class="appearance-none block px-8 py-3 border bg-white border-white leading-tight"
            ><option value="All categories">All categories</option
            ><option value="All categories">All categories</option
            ><option value="All categories">All categories</option>
          </select>
          <div
            class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700"
          >
            <svg
              class="fill-current h-4 w-4"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 20 20"
            >
              <path
                d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"
              />
            </svg>
          </div>
        </div>
        <div class="inline-block relative">
          <select
            name="vendors"
            id=""
            class="appearance-none block px-8 py-3 border bg-white border-white leading-tight"
            ><option class="py-4" value="All categories">All vendors</option
            ><option value="All categories">All categories</option
            ><option value="All categories">All categories</option>
          </select>
          <div
            class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700"
          >
            <svg
              class="fill-current h-4 w-4"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 20 20"
            >
              <path
                d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"
              />
            </svg>
          </div>
        </div>
        <input
          type="text"
          class="py-2 px-8 border-4 border-white"
          placeholder="Search from our list"
        /><button
          class="px-6 py-2 bg-green-600 rounded-r text-white border-4 border-green-600"
        >
          <ion-icon name="search-outline"></ion-icon>
        </button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.prod-header-bg {
  height: 40vh;
  background-image: url('~static/img/products-header-bg.jpg');
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
ion-icon {
  font-size: 20px;
  vertical-align: middle;
  padding-bottom: 3px;
  color: white;
}
</style>

<script>
import Navigation from '@/components/Navigation'
export default {
  components: {
    Navigation
  }
}
</script>
