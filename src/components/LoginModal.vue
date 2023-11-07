<template>
  <Teleport to="body">
    <dialog id="LoginModal" class="modal text-black">
      <div class="modal-box">
        <div>
          <h3 class="flex justify-between items-center">
            <p class="font-semibold text-xl">Welcome to Mart ! Please Login.</p>
            <p class="text-xs">
              New member ?
               <form method="dialog">
        <!-- if there is a button in form, it will close the modal -->
              <button
                class="text-red-700 font-semibold hover:text-red-800"
                onclick="SignupModal.showModal()"
              >
                Sign Up
              </button>
              </form>
            </p>
          </h3>

          <div class="mt-4">
            <label class="text-gray-900">Phone number or Email *</label>
            <input
              class="border p-3 border-gray-300 placeholder:text-gray-400 w-full mt-2"
              placeholder="Please Enter Phone number or email"
            />
          </div>
          <div class="mt-4">
            <label class="text-gray-900">Password *</label>
            <input
              class="border p-3 border-gray-300 placeholder:text-gray-400 w-full mt-2"
              placeholder="Please Enter Phone number or email"
            />
          </div>
          <div class="flex justify-end mt-2">
            <button class="text-orange-400 hover:text-orange-600">
              Reset Password
            </button>
          </div>
          <div class="flex justify-center mt-2">
            <button
              class="hover:scale-125 p-3 w-28 bg-orange-600 rounded-md text-white duration-300"
            >
              Login
            </button>
          </div>
          <div class="divider">OR Login with</div>
          <div class="flex justify-center mt-2">
            <button
              class="hover:bg-blue-950 p-3 w-full bg-blue-900 rounded-md text-white flex items-center justify-center gap-2 text-xl"
            >
              <img
                class="h-8"
                src="https://static.vecteezy.com/system/resources/previews/023/986/613/original/facebook-logo-facebook-logo-transparent-facebook-icon-transparent-free-free-png.png"
              />
              FaceBook
            </button>
          </div>
          <div class="flex justify-center mt-2">
            <button
              class="hover:bg-orange-800 p-3 w-full bg-orange-700 rounded-md text-white flex items-center justify-center gap-2 text-xl"
            >
              <img
                class="h-8"
                src="https://ragsdalemartin.com/wp-content/uploads/2020/07/white-google-logo.png"
              />
              + Google
            </button>
          </div>
        </div>
      </div>
      <form method="dialog" class="modal-backdrop">
        <button>close</button>
      </form>
    </dialog>
  </Teleport>
</template>

<script setup></script>
