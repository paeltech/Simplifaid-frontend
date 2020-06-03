<template>
  <div class="main">
    <div class="flex flex-center justify-around bg-gray-100">
      <div class="w-1/6 bg-gray-900 px-8 py-16">
        <DashboardNav />
      </div>
      <div class="w-5/6 px-8 py-16">
        <DashboardHeader />
        <div class="mt-16 float-right">
          <nuxt-link
            to="/profile/vendors/add"
            class="px-4 py-2 bg-blue-600 text-white font-bold rounded"
          >Add New Vendor</nuxt-link>
        </div>
        <div class="clearfix"></div>
        <h1 class="text-3xl font-bold mt-4">Registered Vendors</h1>
        <table class="w-full rounded-lg shadow-md boder-none mt-6">
          <thead class="bg-gray-300">
            <tr>
              <th class="px-4 py-2 text-left">ID</th>
              <th class="px-4 py-2 text-left">Name</th>
              <th class="px-4 py-2 text-left">Owner</th>
              <th class="px-4 py-2 text-left">Actions</th>
            </tr>
          </thead>
          <tbody v-for="(vendor, index) in vendors" :key="index">
            <tr class="border-b">
              <td class="px-4 py-2 capitalize">{{ index }}</td>
              <td class="px-4 py-2 capitalize">{{ vendor.name }}</td>
              <td class="px-4 py-2 capitalize">{{ vendor.user.name }}</td>
              <td class="px-4 py-2">
                <a href="#" class="mr-2">
                  <ion-icon name="eye-outline"></ion-icon>
                </a>
                <a href="#" class="mr-2">
                  <ion-icon name="create-outline"></ion-icon>
                </a>
                <a href="#" class="mr-2">
                  <ion-icon name="trash-outline"></ion-icon>
                </a>
              </td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
</template>

<script>
import DashboardNav from '@/components/DashboardNav'
import DashboardHeader from '@/components/DashboardHeader'
export default {
  components: {
    DashboardNav,
    DashboardHeader
  },
  data() {
    return {
      vendors: []
    }
  },
  async asyncData({ $axios }) {
    let { data } = await $axios.$get('/vendors')
    return {
      vendors: data
    }
  }
}
</script>

<style scoped>
</style>