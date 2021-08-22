<template>
  <div>
    <div class="conatiner md:px-10 px-2 py-10">
      <div>
        <div class="bg-white rounded-xl p-3 md:p-4 md:w-3/6 md:mx-auto">
          <div>
            <img src="~/assets/image/logo-komfaktek.png" alt="" class="w-48" />
          </div>
          <div class="text-4xl font-bold text-hijau-button mt-4">Register</div>
          <div class="mx-auto mt-6">
            <div class="grid grid-cols-1 md:grid-cols-2 grid-flow-row gap-2">
              <div class="mt-2">
                <div class="mb-2">
                  <label for="email" class="">Nama</label>
                </div>
                <input
                  type="text"
                  class="
                    rounded-full
                    py-1
                    px-2
                    w-full
                    focus:ring-2 focus:ring-hijau-button focus:text-hijau-button
                    border border-gray-500
                    focus:border-transparent focus:outline-none
                  "
                  placeholder="Input Nama"
                />
              </div>
              <div class="mt-2">
                <div class="mb-2">
                  <label for="email" class="">Email</label>
                </div>
                <input
                  type="text"
                  class="
                    rounded-full
                    py-1
                    px-2
                    w-full
                    focus:ring-2 focus:ring-hijau-button focus:text-hijau-button
                    border border-gray-500
                    focus:border-transparent focus:outline-none
                  "
                  placeholder="Input Email"
                />
              </div>
            </div>
            <div
              class="grid grid-cols-1 md:grid-cols-2 grid-flow-row gap-2 mt-4"
            >
              <div class="mt-2">
                <div class="mb-2">
                  <label for="email" class="">Password</label>
                </div>
                <input
                  type="password"
                  class="
                    rounded-full
                    py-1
                    px-2
                    w-full
                    focus:ring-2 focus:ring-hijau-button focus:text-hijau-button
                    border border-gray-500
                    focus:border-transparent focus:outline-none
                  "
                  placeholder="Input Password"
                />
              </div>
              <div class="mt-2">
                <div class="mb-2">
                  <label for="password" class="">Confirm Password</label>
                </div>
                <input
                  type="password"
                  class="
                    rounded-full
                    py-1
                    px-2
                    w-full
                    focus:ring-2 focus:ring-hijau-button focus:text-hijau-button
                    border border-gray-500
                    focus:border-transparent focus:outline-none
                  "
                  placeholder="Input Confirm Password"
                />
              </div>
            </div>
            <div class="w-full mt-8">
              <a
                href="index.html"
                class="
                  bg-hijau-button
                  py-2
                  block
                  text-center text-white
                  rounded-full
                  hover:bg-hijau-header
                "
                >Register</a
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
