<template>
  <div>
    <navmobile />
    <div class="bg-gradient-to-r from-green-500 px-4 to-green-800 py-4 pb-6">
      <div>
        <img
          :src="this.$store.state.auth.user.user_detail.image"
          class="
            rounded-full
            border-2 border-white
            w-24
            h-24
            object-cover
            mx-auto
          "
          alt=""
        />
      </div>
      <div class="mt-4 text-center">
        <div class="text-white text-lg font-medium">
          {{ this.$store.state.auth.user.name }}
        </div>
        <div class="text-gray-300">
          {{ this.$store.state.auth.user.user_detail.profesi }}
        </div>
      </div>
    </div>
    <div class="px-4 bg-white py-6 -mt-4 rounded-t-2xl">
      <nuxt-link to="/dashboard/profile">
        <div class="flex mb-8">
          <div>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-7 w-7 text-gray-800"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"
              />
            </svg>
          </div>
          <div class="my-auto">
            <div class="text-gray-800 text-lg ml-4">Profile</div>
          </div>
        </div>
      </nuxt-link>

      <nuxt-link to="/dashboard/event-saya">
        <div class="flex mb-8">
          <div>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-7 w-7 text-gray-800"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z"
              />
            </svg>
          </div>
          <div class="my-auto">
            <div class="text-gray-800 text-lg ml-4">Event saya</div>
          </div>
        </div>
      </nuxt-link>

      <div class="flex mb-8">
        <div>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-7 w-7 text-gray-800"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z"
            />
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"
            />
          </svg>
        </div>
        <div class="my-auto">
          <div class="text-gray-800 text-lg ml-4">Pengaturan akun</div>
        </div>
      </div>
      <div class="flex mb-8 cursor-pointer" @click="userLogout">
        <div>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-7 w-7 text-gray-800"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M17 16l4-4m0 0l-4-4m4 4H7m6 4v1a3 3 0 01-3 3H6a3 3 0 01-3-3V7a3 3 0 013-3h4a3 3 0 013 3v1"
            />
          </svg>
        </div>
        <div class="my-auto">
          <div class="text-gray-800 text-lg ml-4">Logout</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  middleware: 'auth',
  data() {
    return {}
  },
  mounted() {},
  methods: {
    async userLogout() {
      await this.$auth.logout()
    },
  },
}
</script>
