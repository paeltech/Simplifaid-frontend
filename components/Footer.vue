<template>
  <div class="container mx-auto mt-32 px-6">
    <hr />
    <div class="flex flex-col md:justify-between mt-16 pb-8 md:pb-16">
      <div class="w-full md:w-1/2">
        <h4 class="text-2xl font-bold">Let's get social</h4>
        <ul class="flex flex-row item-start mt-4">
          <li>
            <a class="mr-4" href="#">
              <ion-icon name="logo-facebook"></ion-icon>Facebook
            </a>
          </li>
          <li>
            <a class="mr-4" href="#">
              <ion-icon name="logo-twitter"></ion-icon>Twitter
            </a>
          </li>
          <li>
            <a class="mr-4" href="#">
              <ion-icon name="logo-instagram"></ion-icon>Instagram
            </a>
          </li>
        </ul>
      </div>

      <div class="w-full md:w-1/2">
        <p class="md:float-right md:mt-8 pt-6">
          &copy; Simplifaid | A product of
          <a href="#">Hawks.agency</a>
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
ion-icon {
  font-size: 24px;
  vertical-align: middle;
  padding-bottom: 3px;
}
</style>
