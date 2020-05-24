<template>
  <div>
    <div class="container mx-auto p-6">
      <Navigation />
    </div>
    <div class="container mx-auto p-6">
      <section id="hero-section">
        <div class="flex flex-row content-center justify-between">
          <div class="w-5/12">
            <h1 class="text-4xl font-bold">You don’t have to panic, Everything is simplifaid.</h1>
            <p class="pt-4">
              Because of the current situation, everyone is worried to move form
              their homes but we still need to eat so we can live. Simplifaid
              exists to help you get your groceries at your door step. All you
              have to do is place an order and we deliver.
            </p>
            <div class="mt-12">
              <nuxt-link
                class="px-8 py-4 bg-green-600 text-white hover:bg-green-500 font-bold rounded"
                to="/products"
              >SHOP NOW</nuxt-link>
            </div>
          </div>
          <div class="w-5/12">
            <img class="float-right header-img" src="~/static/img/header-img.png" alt />
          </div>
        </div>
      </section>
      <section id="categories-section" class="mt-32">
        <div class="text-center">
          <h2 class="text-3xl font-bold">Product categories</h2>
          <p class="text-green-600 text-sm">
            Categories of products that you can
            <br />order through our platform.
          </p>
        </div>
        <div class="grid gap-8 grid-cols-4 mt-24">
          <div>
            <div class="px-6 py-8 bg-gray-100 rounded">
              <img src="~/static/img/fruits.png" alt />
              <h3 class="pt-6 font-bold text-center text-2xl mb-4">Fruits</h3>
            </div>
          </div>
          <div>
            <div class="px-6 py-8 bg-gray-100 rounded">
              <img src="~/static/img/cereals.png" alt />
              <h3 class="pt-6 font-bold text-center text-2xl mb-4">Cereals</h3>
            </div>
          </div>
          <div>
            <div class="px-6 py-8 bg-gray-100 rounded">
              <img src="~/static/img/herbs.png" alt />
              <h3 class="pt-6 font-bold text-center text-2xl mb-4">Herbs</h3>
            </div>
          </div>
          <div>
            <div class="px-6 py-8 bg-gray-100 rounded">
              <img src="~/static/img/meat.png" alt />
              <h3 class="pt-6 font-bold text-center text-2xl mb-4">Meat</h3>
            </div>
          </div>
        </div>
      </section>
      <section id="process-section" class="mt-32">
        <div class="text-center">
          <h2 class="text-3xl font-bold">How it works</h2>
          <p class="text-green-600 text-sm">
            In three steps you will be done,
            <br />just waiting for your delivery.
          </p>
        </div>
        <div class="w-2/3 mx-auto grid gap-8 grid-cols-3 mt-24">
          <div>
            <div class="flex flex-col items-center justify-center px-10 py-16 bg-gray-100 rounded">
              <div
                class="flex items-center justify-center w-16 h-16 border border-green-600 rounded-full text-3xl font-bold"
              >
                <ion-icon name="search-sharp"></ion-icon>
              </div>
              <h3 class="pt-6 text-center mb-4">
                Select items of
                <br />choice
              </h3>
            </div>
          </div>
          <div>
            <div class="flex flex-col items-center justify-center px-10 py-16 bg-gray-100 rounded">
              <div
                class="flex items-center justify-center w-16 h-16 border border-green-600 rounded-full text-3xl font-bold"
              >
                <ion-icon name="add-sharp"></ion-icon>
              </div>
              <h3 class="pt-6 text-center mb-4">
                Add to your
                <br />basket
              </h3>
            </div>
          </div>
          <div>
            <div class="flex flex-col items-center justify-center px-10 py-16 bg-gray-100 rounded">
              <div
                class="flex items-center justify-center w-16 h-16 border border-green-600 rounded-full text-3xl font-bold"
              >
                <ion-icon name="checkmark-sharp"></ion-icon>
              </div>
              <h3 class="pt-6 text-center mb-4">
                Place your
                <br />order
              </h3>
            </div>
          </div>
        </div>
      </section>
    </div>
    <Footer />
  </div>
</template>

<style scoped>
.header-img {
  width: 90%;
}
</style>

<script>
import Navigation from '@/components/Navigation'
import Footer from '@/components/Footer'
export default {
  components: {
    Navigation,
    Footer
  }
  //middleware: ['auth']
}
</script>
