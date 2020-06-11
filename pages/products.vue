<template>
  <div>
    <SubNav />
    <section id="kids-special" class="container mx-auto p-6 mt-12">
      <div class="bg-white rounded-md px-6 md:px-12 py-8">
        <div class>
          <span class="float-right">
            I don't need this
            <span class="text-green-600">X</span>
          </span>
          <p class="text-green-600">Special</p>
          <h1 class="text-2xl">FOR CHILDREN</h1>
        </div>
        <div class="grid gap-4 md:gap-8 grid-cols-2 md:grid-cols-4 mt-6">
          <div>
            <div class="hover:bg-gray-100 rounded">
              <img class="px-2 md:px-6 pt" src="~/static/img/fruits.png" alt />
              <div class="px-4 pb-4">
                <h2 class="pt-2 font-bol text-center text-xl text-gray-800 mb">Tomatoes</h2>
                <p class="pt-0 text-sm text-center">
                  <span class="font-bold">1300</span>Tsh/Kg
                </p>
              </div>
              <div :class="isOpen ? 'block' : 'hidden'" class="text-center">
                <span class="shadow px-3 py-2 pt-4">
                  <a href="#" @click.prevent="removeUnits" class="text-green-600 text-2xl">
                    <ion-icon name="remove-circle-outline"></ion-icon>
                  </a>
                  <a href="#" v-if="trash" @click.prevent="removeUnits">T</a>
                  <span class="text-xl px-4">{{ units }}</span>
                  <a href="#" @click.prevent="addUnits" class="text-green-600 text-2xl">
                    <ion-icon name="add-circle-outline"></ion-icon>
                  </a>
                </span>
              </div>

              <div
                @click="addUnits, isOpen=true, addButton=false"
                :class="addButton ? 'block' : 'hidden'"
                class="text-green-600 text-2xl text-center"
              >
                <ion-icon name="add-circle-outline"></ion-icon>
              </div>
            </div>
          </div>
          <div>
            <div class="hover:bg-gray-100 rounded">
              <img class="px-6 pt" src="~/static/img/herbs.png" alt />
              <div class="px-4 pb-4">
                <h2 class="pt-2 font-bol text-center text-xl text-gray-800 mb">Corriander</h2>
                <p class="pt-0 text-sm text-center">
                  <span class="font-bold">1300</span>Tsh/Kg
                </p>
              </div>
              <div :class="isOpen ? 'block' : 'hidden'" class="text-center">
                <span class="shadow px-3 py-2 pt-4">
                  <a href="#" @click.prevent="removeUnits" class="text-green-600 text-2xl">
                    <ion-icon name="remove-circle-outline"></ion-icon>
                  </a>
                  <a href="#" v-if="trash" @click.prevent="removeUnits">T</a>
                  <span class="text-xl px-4">{{ units }}</span>
                  <a href="#" @click.prevent="addUnits" class="text-green-600 text-2xl">
                    <ion-icon name="add-circle-outline"></ion-icon>
                  </a>
                </span>
              </div>

              <div
                @click="addUnits, isOpen=true, addButton=false"
                :class="addButton ? 'block' : 'hidden'"
                class="text-green-600 text-2xl text-center"
              >
                <ion-icon name="add-circle-outline"></ion-icon>
              </div>
            </div>
          </div>
          <div>
            <div class="hover:bg-gray-100 rounded">
              <img class="px-6 pt" src="~/static/img/cereals.png" alt />
              <div class="px-4 pb-4">
                <h2 class="pt-2 font-bol text-center text-xl text-gray-800 mb">Cereals</h2>
                <p class="pt-0 text-sm text-center">
                  <span class="font-bold">1300</span>Tsh/Kg
                </p>
              </div>
              <div :class="isOpen ? 'block' : 'hidden'" class="text-center">
                <span class="shadow px-3 py-2 pt-4">
                  <a href="#" @click.prevent="removeUnits" class="text-green-600 text-2xl">
                    <ion-icon name="remove-circle-outline"></ion-icon>
                  </a>
                  <a href="#" v-if="trash" @click.prevent="removeUnits">T</a>
                  <span class="text-xl px-4">{{ units }}</span>
                  <a href="#" @click.prevent="addUnits" class="text-green-600 text-2xl">
                    <ion-icon name="add-circle-outline"></ion-icon>
                  </a>
                </span>
              </div>

              <div
                @click="addUnits, isOpen=true, addButton=false"
                :class="addButton ? 'block' : 'hidden'"
                class="text-green-600 text-2xl text-center"
              >
                <ion-icon name="add-circle-outline"></ion-icon>
              </div>
            </div>
          </div>
          <div>
            <div class="hover:bg-gray-100 rounded">
              <img class="px-6 pt" src="~/static/img/meat.png" alt />
              <div class="px-4 pb-4">
                <h2 class="pt-2 font-bol text-center text-xl text-gray-800 mb">Meat</h2>
                <p class="pt-0 text-sm text-center">
                  <span class="font-bold">1300</span>Tsh/Kg
                </p>
              </div>
              <div :class="isOpen ? 'block' : 'hidden'" class="text-center">
                <span class="shadow px-3 py-2 pt-4">
                  <a href="#" @click.prevent="removeUnits" class="text-green-600 text-2xl">
                    <ion-icon name="remove-circle-outline"></ion-icon>
                  </a>
                  <a href="#" v-if="trash" @click.prevent="removeUnits">T</a>
                  <span class="text-xl px-4">{{ units }}</span>
                  <a href="#" @click.prevent="addUnits" class="text-green-600 text-2xl">
                    <ion-icon name="add-circle-outline"></ion-icon>
                  </a>
                </span>
              </div>

              <div
                @click="addUnits, isOpen=true, addButton=false"
                :class="addButton ? 'block' : 'hidden'"
                class="text-green-600 text-2xl text-center"
              >
                <ion-icon name="add-circle-outline"></ion-icon>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section id="kids-special" class="container mx-auto p-6">
      <div class="px-6 md:px-12 py-8">
        <div class>
          <p class="text-green-600">Fresh</p>
          <h1 class="text-2xl">VEGETABLES</h1>
        </div>
        <div class="grid gap-4 md:gap-8 grid-cols-2 md:grid-cols-4 mt-6">
          <div>
            <div class="hover:bg-gray-100 pb-2 rounded">
              <img class="px-4 md:px-6 pt" src="~/static/img/fruits.png" alt />
              <div class="px-4 pb-4">
                <h2 class="pt-2 font-bol text-center text-xl text-gray-800 mb">Tomatoes</h2>
                <p class="pt-0 text-sm text-center">
                  <span class="font-bold">1300</span>Tsh/Kg
                </p>
              </div>
              <div :class="isOpen ? 'block' : 'hidden'" class="text-center">
                <span class="shadow px-3 py-2 pt-4">
                  <a href="#" @click.prevent="removeUnits" class="text-green-600 text-2xl">
                    <ion-icon name="remove-circle-outline"></ion-icon>
                  </a>
                  <a href="#" v-if="trash" @click.prevent="removeUnits">T</a>
                  <span class="text-xl px-4">{{ units }}</span>
                  <a href="#" @click.prevent="addUnits" class="text-green-600 text-2xl">
                    <ion-icon name="add-circle-outline"></ion-icon>
                  </a>
                </span>
              </div>

              <div
                @click="addUnits, isOpen=true, addButton=false"
                :class="addButton ? 'block' : 'hidden'"
                class="text-green-600 text-2xl text-center"
              >
                <ion-icon name="add-circle-outline"></ion-icon>
              </div>
            </div>
          </div>
          <div>
            <div class="hover:bg-gray-100 pb-2 rounded">
              <img class="px-4 md:px-6 pt" src="~/static/img/herbs.png" alt />
              <div class="px-4 pb-4">
                <h2 class="pt-2 font-bol text-center text-xl text-gray-800 mb">Corriander</h2>
                <p class="pt-0 text-sm text-center">
                  <span class="font-bold">1300</span>Tsh/Kg
                </p>
              </div>
              <div :class="isOpen ? 'block' : 'hidden'" class="text-center">
                <span class="shadow px-3 py-2 pt-4">
                  <a href="#" @click.prevent="removeUnits" class="text-green-600 text-2xl">
                    <ion-icon name="remove-circle-outline"></ion-icon>
                  </a>
                  <a href="#" v-if="trash" @click.prevent="removeUnits">T</a>
                  <span class="text-xl px-4">{{ units }}</span>
                  <a href="#" @click.prevent="addUnits" class="text-green-600 text-2xl">
                    <ion-icon name="add-circle-outline"></ion-icon>
                  </a>
                </span>
              </div>

              <div
                @click="addUnits, isOpen=true, addButton=false"
                :class="addButton ? 'block' : 'hidden'"
                class="text-green-600 text-2xl text-center"
              >
                <ion-icon name="add-circle-outline"></ion-icon>
              </div>
            </div>
          </div>
          <div>
            <div class="hover:bg-gray-100 rounded">
              <img class="px-6 pt" src="~/static/img/cereals.png" alt />
              <div class="px-4 pb-4">
                <h2 class="pt-2 font-bol text-center text-xl text-gray-800 mb">Cereals</h2>
                <p class="pt-0 text-sm text-center">
                  <span class="font-bold">1300</span>Tsh/Kg
                </p>
              </div>
              <div :class="isOpen ? 'block' : 'hidden'" class="text-center">
                <span class="shadow px-3 py-2 pt-4">
                  <a href="#" @click.prevent="removeUnits" class="text-green-600 text-2xl">
                    <ion-icon name="remove-circle-outline"></ion-icon>
                  </a>
                  <a href="#" v-if="trash" @click.prevent="removeUnits">T</a>
                  <span class="text-xl px-4">{{ units }}</span>
                  <a href="#" @click.prevent="addUnits" class="text-green-600 text-2xl">
                    <ion-icon name="add-circle-outline"></ion-icon>
                  </a>
                </span>
              </div>

              <div
                @click="addUnits, isOpen=true, addButton=false"
                :class="addButton ? 'block' : 'hidden'"
                class="text-green-600 text-2xl text-center"
              >
                <ion-icon name="add-circle-outline"></ion-icon>
              </div>
            </div>
          </div>
          <div>
            <div class="hover:bg-gray-100 rounded">
              <img class="px-6 pt" src="~/static/img/meat.png" alt />
              <div class="px-4 pb-4">
                <h2 class="pt-2 font-bol text-center text-xl text-gray-800 mb">Meat</h2>
                <p class="pt-0 text-sm text-center">
                  <span class="font-bold">1300</span>Tsh/Kg
                </p>
              </div>
              <div :class="isOpen ? 'block' : 'hidden'" class="text-center">
                <span class="shadow px-3 py-2 pt-4">
                  <a href="#" @click.prevent="removeUnits" class="text-green-600 text-2xl">
                    <ion-icon name="remove-circle-outline"></ion-icon>
                  </a>
                  <a href="#" v-if="trash" @click.prevent="removeUnits">T</a>
                  <span class="text-xl px-4">{{ units }}</span>
                  <a href="#" @click.prevent="addUnits" class="text-green-600 text-2xl">
                    <ion-icon name="add-circle-outline"></ion-icon>
                  </a>
                </span>
              </div>

              <div
                @click="addUnits, isOpen=true, addButton=false"
                :class="addButton ? 'block' : 'hidden'"
                class="text-green-600 text-2xl text-center"
              >
                <ion-icon name="add-circle-outline"></ion-icon>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <Footer />
  </div>
</template>

<style scoped>
ion-icon {
  vertical-align: middle;
  padding-bottom: 3px;
}
</style>
<script>
import SubNav from '@/components/SubNav'
import Footer from '@/components/Footer'
export default {
  data() {
    return {
      isOpen: false,
      addButton: true,
      trash: false,
      units: 0
    }
  },
  components: {
    SubNav,
    Footer
  },
  methods: {
    addUnits: function() {
      this.units += 1
    },
    removeUnits: function() {
      this.units -= 1
    },
    displayTrash: function() {
      if (this.units == 1) {
        trash: true
      }
    }
  }
}
</script>
