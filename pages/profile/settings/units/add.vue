<template>
  <div>
    <div class="container mx-auto w-1/1 flex flex-col content-center justify-center">
      <div class="px-8 py-16 rounded-lg bg-white mt-32 mb-16">
        <h3 class="text-2xl font-bold mb-4">Product Measurement Units</h3>

        <form @submit.prevent="create">
          <div class="mb-4">
            <label class="block text-gray-800 text-sm font-bold mb-2" for="unit">Unit</label>
            <input
              v-model.trim="form.name"
              class="appearance-none border border-gray-500 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
              id="unit"
              type="text"
              placeholder="Unit measure eg. Kg"
              autofocus
            />
            <small v-if="errors.name" class="mt-2 text-red-500">{{ errors.name[0] }}</small>
          </div>

          <div class="flex items-center justify-between">
            <button
              class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline"
              type="submit"
              value="submit"
            >Create unit</button>
          </div>
        </form>
      </div>
    </div>
    <Units />
  </div>
</template>

<script>
import Units from '@/components/Units'
export default {
  middleware: ['auth'],
  components: {
    Units
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
      await this.$axios.$post('/units', this.form)
      this.$router.push({
        path: this.$route.query.redirect || '/profile/settings/units'
      })
    }
  }
}
</script>

<style lang="scss" scoped>
</style>