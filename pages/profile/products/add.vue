<template>
  <div class="main">
    <div class="flex flex-center justify-around bg-gray-100">
      <div class="w-1/6 bg-gray-900 px-8 py-16">
        <DashboardNav />
      </div>
      <div class="w-5/6 px-8 py-16">
        <DashboardHeader />
        <h1 class="mt-16 text-3xl font-bold">Register New Vendor</h1>
        <form @submit.prevent="create" class="w-3/4 mt-6">
          <div class="mb-4">
            <label class="block text-gray-800 text-xl font-bold mb-2" for="name">Vendor Name</label>
            <input
              v-model.trim="form.name"
              class="appearance-none border border-gray-500 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
              id="name"
              type="text"
              placeholder="Name of the vendor"
              autofocus
            />
            <small v-if="errors.name" class="mt-2 text-red-500">{{ errors.name[0] }}</small>
          </div>
          <div class="mb-4">
            <label class="block text-gray-800 text-xl font-bold mb-2" for="avatar">Avatar</label>
            <input
              v-model.trim="form.avatar"
              class="appearance-none border border-gray-500 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
              id="avatar"
              type="text"
              placeholder="Name of the vendor"
              autofocus
            />
            <small v-if="errors.name" class="mt-2 text-red-500">{{ errors.name[0] }}</small>
          </div>

          <div class="flex items-center justify-between">
            <button
              class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline"
              type="submit"
              value="submit"
            >Create vendor account</button>
          </div>
        </form>
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
      form: {
        name: ''
      }
    }
  },
  methods: {
    async create() {
      await this.$axios.$post('/vendors', this.form)
      this.$router.push({
        path: this.$route.query.redirect || '/profile'
      })
    }
  }
}
</script>

<style scoped>
</style>