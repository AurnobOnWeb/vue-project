<template>
  <div class="flex justify-between text-sm h-4">
    <div>
      <button class="hover:text-gray-300 mr-2">Become a Seller</button>
      <button class="hover:text-gray-300 ml-2">Help & Support</button>
    </div>
    <div>
      <button
        class="bg-orange-800 px-4 py-1 shadow-md rounded-b-lg hover:bg-orange-900 transition-colors duration-200 flex items-center gap-2"
        onclick="my_modal_2.showModal()"
      >
        <img
          class="h-4"
          src="https://www.pngkit.com/png/full/85-857608_friendstv-club-friends-logo-white-png.png"
        />
        Download App
      </button>
      <Teleport to="body">
        <dialog id="my_modal_2" class="modal">
          <div class="modal-box">
            <h3 class="font-bold text-lg flex justify-center">
              Scan To Download!
            </h3>
            <img
              class="flex justify-center p-2 ml-3"
              src="https://www.techopedia.com/wp-content/uploads/2023/03/aee977ce-f946-4451-8b9e-bba278ba5f13.png"
            />
          </div>
          <form method="dialog" class="modal-backdrop">
            <button>close</button>
          </form>
        </dialog>
      </Teleport>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
