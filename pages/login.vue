<template>
  <div>
    <div
      class="container mx-auto w-3/4 md:w-1/4 h-full flex flex-col content-center justify-center"
    >
      <div class="px-8 py-16 rounded-lg bg-white mt-16 md:mt-32 mb-32">
        <h3 class="text-2xl font-bold mb-4">Login</h3>

        <form @submit.prevent="pressed">
          <div class="mb-4">
            <label class="block text-gray-800 text-sm font-bold mb-2" for="email">Email</label>
            <input
              v-model.trim="form.email"
              class="appearance-none border border-gray-500 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
              id="email"
              type="text"
              placeholder="Email"
              autofocus
            />
            <small v-if="errors.email" class="mt-2 text-red-500">{{ errors.email[0] }}</small>
          </div>
          <div class="mb-6">
            <label class="block text-gray-800 text-sm font-bold mb-2" for="password">Password</label>
            <input
              v-model.trim="form.password"
              class="appearance-none border border-gray-500 rounded w-full py-2 px-3 text-gray-700 mb-3 leading-tight focus:outline-none focus:shadow-outline"
              id="password"
              type="password"
              placeholder="******************"
            />
            <small v-if="errors.password" class="mt-2 text-red-500">{{ errors.password[0] }}</small>
          </div>
          <div class="flex items-center justify-between">
            <button
              class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline"
              type="submit"
              value="submit"
            >Sign In</button>
            <a
              class="inline-block align-baseline font-bold text-sm text-blue-500 hover:text-blue-800"
              href="#"
            >Forgot Password?</a>
          </div>
          <div class="mt-6 text-gray-800">
            <p>
              Don't have an account?
              <nuxt-link to="/register" class="text-blue-500">Register</nuxt-link>
            </p>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  middleware: ['guest'],
  data() {
    return {
      form: {
        email: '',
        password: ''
      }
    }
  },
  methods: {
    async pressed() {
      try {
        await this.$auth.loginWith('local', {
          data: this.form
        }),
          this.$router.push({
            path: this.$route.query.redirect || '/profile'
          })
      } catch (e) {
        return
      }
    }
  }
}
</script>

<style scoped>
</style>
