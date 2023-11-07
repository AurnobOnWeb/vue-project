<template>
  <div class="w-full h-auto bg-orange-600 text-white lg:flex lg:justify-center">
    <div class="lg:w-[80%] xl:w-[70%] h-24 mx-2 lg:mx-0">
      <TopHeader />
      <div class="h-18 mt-2">
        <div class="flex flex-row justify-between items-center gap-4">
          <div class="w-full flex items-center">
            <img
              class="h-16 p-1"
              src="https://icms-image.slatic.net/images/ims-web/3ac46ea5-a376-41cc-981f-21fa690468c0.png"
              alt="logo"
            />

            <div class="flex w-full">
              <div class="relative w-full">
                <input
                  type="search"
                  id="search-dropdown"
                  class="block p-2.5 z-20 w-full text-sm text-gray-900 bg-gray-50 rounded-r-lg border-l-gray-50 border-l-2 border border-gray-300 focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-l-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:border-blue-500"
                  placeholder="Search Mockups, Logos, Design Templates..."
                  required
                />
                <button
                  type="submit"
                  class="absolute top-0 right-0 p-2.5 h-full text-white bg-blue-700 rounded-r-lg border border-blue-700 hover:bg-blue-800 dark:bg-blue-600 dark:hover:bg-blue-700"
                >
                  <svg
                    class="w-4 h-4"
                    aria-hidden="true"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 20 20"
                  >
                    <path
                      stroke="currentColor"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="m19 19-4-4m0-7A7 7 0 1 1 1 8a7 7 0 0 1 14 0Z"
                    />
                  </svg>
                  <span class="sr-only">Search</span>
                </button>
              </div>
            </div>
          </div>

          <div class="flex items-center justify-center">
            <button
              class="font-bold mr-1 text-xl"
              onclick="LoginModal.showModal()"
            >
              Login
            </button>
            <LoginModal />
            |
            <button
              class="font-bold ml-1 text-xl"
              onclick="SignupModal.showModal()"
            >
              SignUp
            </button>
            <SignupModal />
            <button class="">
              <img
                src="https://svgsilh.com/svg/294547.svg"
                class="h-20 w-28 md:w-20"
                alt="cart"
              />
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import LoginModal from "../components/LoginModal.vue";
import SignupModal from "../components/SignupModal.vue";
import TopHeader from "../components/TopHeader.vue";
</script>

<style lang="scss" scoped></style>
