<template>
  <div class="main">
    <div class="flex flex-center justify-around bg-gray-100">
      <div class="w-1/6 bg-gray-900 px-8 py-16">
        <DashboardNav />
      </div>
      <div class="w-5/6 px-8 py-16">
        <DashboardHeader />
        <section class="widgets-area w-full">
          <div class="grid gap-8 grid-cols-5 mt-6">
            <div>
              <div class="rounded h-full flex justify-center items-center">
                <div class="rounded bg-white shadow-md h-48 w-48 p-6 flex flex-col justify-around">
                  <div>
                    <p class="text-base text-gray-600">Revenue</p>
                  </div>
                  <div>
                    <p class="text-2xl text-gray-700 font-bold">$56,734</p>
                  </div>
                  <div class="text-sm">
                    <p class="text-green-500 mb-1 flex item-center">
                      <i class="material-icons">arrow_drop_up</i>
                      5.77%
                    </p>
                    <p class="text-gray-600">Since last month</p>
                  </div>
                </div>
              </div>
            </div>
            <div>
              <div class="rounded h-full flex justify-center items-center">
                <div class="rounded bg-white shadow-md h-48 w-48 p-6 flex flex-col justify-around">
                  <div>
                    <p class="text-base text-gray-600">Revenue</p>
                  </div>
                  <div>
                    <p class="text-2xl text-gray-700 font-bold">$56,734</p>
                  </div>
                  <div class="text-sm">
                    <p class="text-green-500 mb-1 flex item-center">
                      <i class="material-icons">arrow_drop_up</i>
                      5.77%
                    </p>
                    <p class="text-gray-600">Since last month</p>
                  </div>
                </div>
              </div>
            </div>
            <div>
              <div class="rounded h-full flex justify-center items-center">
                <div class="rounded bg-white shadow-md h-48 w-48 p-6 flex flex-col justify-around">
                  <div>
                    <p class="text-base text-gray-600">Revenue</p>
                  </div>
                  <div>
                    <p class="text-2xl text-gray-700 font-bold">$56,734</p>
                  </div>
                  <div class="text-sm">
                    <p class="text-green-500 mb-1 flex item-center">
                      <i class="material-icons">arrow_drop_up</i>
                      5.77%
                    </p>
                    <p class="text-gray-600">Since last month</p>
                  </div>
                </div>
              </div>
            </div>
            <div>
              <div class="rounded h-full flex justify-center items-center">
                <div class="rounded bg-white shadow-md h-48 w-48 p-6 flex flex-col justify-around">
                  <div>
                    <p class="text-base text-gray-600">Revenue</p>
                  </div>
                  <div>
                    <p class="text-2xl text-gray-700 font-bold">$56,734</p>
                  </div>
                  <div class="text-sm">
                    <p class="text-green-500 mb-1 flex item-center">
                      <i class="material-icons">arrow_drop_up</i>
                      5.77%
                    </p>
                    <p class="text-gray-600">Since last month</p>
                  </div>
                </div>
              </div>
            </div>
            <div>
              <div class="rounded h-full flex justify-center items-center">
                <div class="rounded bg-white shadow-md h-48 w-48 p-6 flex flex-col justify-around">
                  <div>
                    <p class="text-base text-gray-600">Revenue</p>
                  </div>
                  <div>
                    <p class="text-2xl text-gray-700 font-bold">$56,734</p>
                  </div>
                  <div class="text-sm">
                    <p class="text-green-500 mb-1 flex item-center">
                      <i class="material-icons">arrow_drop_up</i>
                      5.77%
                    </p>
                    <p class="text-gray-600">Since last month</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>
        <section class="data-table">
          <h2 class="text-3xl font-bold mt-16">Incoming Orders</h2>
          <table class="w-full rounded-lg shadow-md boder-none mt-6">
            <thead class="bg-gray-300">
              <tr>
                <th class="px-4 py-2">Order ID</th>
                <th class="px-4 py-2">Amount</th>
                <th class="px-4 py-2">Store</th>
                <th class="px-4 py-2">Shipping adress</th>
                <th class="px-4 py-2">Customer mobile</th>
                <th class="px-4 py-2">Status</th>
                <th class="px-4 py-2">Actions</th>
              </tr>
            </thead>
            <tbody>
              <tr class="border-b">
                <td class="px-4 py-2">843759AB3</td>
                <td class="px-4 py-2">42,000TZS</td>
                <td class="px-4 py-2">Simplifaid plus</td>
                <td class="px-4 py-2">Kawe, kwa warioba</td>
                <td class="px-4 py-2">0756786573</td>
                <td class="px-4 py-2">Pending</td>
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
              <tr class="border-b">
                <td class="px-4 py-2">843759AB3</td>
                <td class="px-4 py-2">42,000TZS</td>
                <td class="px-4 py-2">Simplifaid plus</td>
                <td class="px-4 py-2">Kawe, kwa warioba</td>
                <td class="px-4 py-2">0756786573</td>
                <td class="px-4 py-2">Pending</td>
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
              <tr class="border-b">
                <td class="px-4 py-2">843759AB3</td>
                <td class="px-4 py-2">42,000TZS</td>
                <td class="px-4 py-2">Simplifaid plus</td>
                <td class="px-4 py-2">Kawe, kwa warioba</td>
                <td class="px-4 py-2">0756786573</td>
                <td class="px-4 py-2">Pending</td>
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
              <tr class="border-b">
                <td class="px-4 py-2">843759AB3</td>
                <td class="px-4 py-2">42,000TZS</td>
                <td class="px-4 py-2">Simplifaid plus</td>
                <td class="px-4 py-2">Kawe, kwa warioba</td>
                <td class="px-4 py-2">0756786573</td>
                <td class="px-4 py-2">Pending</td>
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
              <tr class="border-b">
                <td class="px-4 py-2">843759AB3</td>
                <td class="px-4 py-2">42,000TZS</td>
                <td class="px-4 py-2">Simplifaid plus</td>
                <td class="px-4 py-2">Kawe, kwa warioba</td>
                <td class="px-4 py-2">0756786573</td>
                <td class="px-4 py-2">Pending</td>
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
              <tr class="border-b">
                <td class="px-4 py-2">843759AB3</td>
                <td class="px-4 py-2">42,000TZS</td>
                <td class="px-4 py-2">Simplifaid plus</td>
                <td class="px-4 py-2">Kawe, kwa warioba</td>
                <td class="px-4 py-2">0756786573</td>
                <td class="px-4 py-2">Pending</td>
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
              <tr class="border-b">
                <td class="px-4 py-2">843759AB3</td>
                <td class="px-4 py-2">42,000TZS</td>
                <td class="px-4 py-2">Simplifaid plus</td>
                <td class="px-4 py-2">Kawe, kwa warioba</td>
                <td class="px-4 py-2">0756786573</td>
                <td class="px-4 py-2">Pending</td>
                <td class="px-4 py-2">
                  <a href="#" class="mr-2 hover:text-red-600">
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
        </section>
        <footer class="footer-nav">
          <p class="text-center mt-16">
            Powered by
            <a href="hawks.agency">hawks.agency</a>
          </p>
        </footer>
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
  }
}
</script>

<style scoped>
.main {
  height: 100vh;
}
th {
  border: 0;
}
ion-icon {
  width: 16px;
}

.menu ion-icon {
  width: 22px;
  color: aliceblue;
}
</style>