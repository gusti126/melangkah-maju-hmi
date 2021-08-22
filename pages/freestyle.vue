<template>
  <div class="">
    <div class="p-4 bg-white rounded-lg">
      <div class="text-2xl font-semibold mb-2">Tava Restaurant</div>
      <div class="flex">
        <img
          src="~assets/freestyle/location.png"
          alt=""
          class="mb-4 w-5 mr-2"
        />
        <div class="text-gray-600 text-sm">Pamulang, Tangerang Selatan</div>
      </div>
      <img
        src="~/assets/freestyle/Rectangle 387.png"
        alt=""
        class="rounded-lg"
      />
      <div class="mt-4 flex justify-between">
        <div>
          <div class="flex">
            <img src="~/assets/freestyle/jam.png" alt="" class="mr-2 w-5" />
            <div>
              <div class="my-auto text-xs text-gray-600">Open To Day</div>
            </div>
          </div>
          <div class="font-medium">10.00 AM - 12.00 PM</div>
        </div>
        <div class="flex my-auto">
          <img src="~/assets/freestyle/visit.png" alt="" class="w-6 h-6 mr-2" />
          <div class="text-xs my-auto text-blue-600">Visit teh Restaurant</div>
        </div>
      </div>
    </div>
    <div class="bg-white py-4 mt-4 px-4">
      <div class="flex justify-between mb-4">
        <div>
          <div class="font-semibold text-xl">List other</div>
          <div class="text-xs text-gray-500">
            check the menu at this restaurant
          </div>
        </div>
        <div class="text-green-500 text-lg font-medium my-auto">See all</div>
      </div>
      <div
        class="border p-2 mb-4 rounded-lg flex justify-between"
        v-for="p of 4"
      >
        <div>
          <img src="~/assets/freestyle/Rectangle 3.png" alt="" class="w-14" />
        </div>
        <div>
          <div class="text-xl font-medium">Ambrosia Hotel</div>
          <div class="flex justify-items-center">
            <div class="my-auto">
              <img
                src="~assets/freestyle/location.png"
                alt=""
                class="w-5 mt-2 mr-2 my-auto"
              />
            </div>
            <div class="my-auto text-sm">Jakarta Barat</div>
          </div>
        </div>
        <div class="my-auto">
          <div class="bg-green-600 text-white px-4 py-2 rounded-lg my-auto">
            Check
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
