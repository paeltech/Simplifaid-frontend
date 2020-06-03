<template>
  <div class="container mx-auto mt-10 rounded-lg bg-white p-8 mb-32">
    <h1 class="text-2xl font-bold mb-4">Available Product Units</h1>
    <div v-for="(unit, index) in units" :key="index">
      <h3>{{ unit.name }}</h3>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      units: []
    }
  },
  async asyncData({ $axios }) {
    let { data } = await $axios.$get('/units/')
    return {
      units: data
    }
  }
}
</script>

<style lang="scss" scoped>
</style>