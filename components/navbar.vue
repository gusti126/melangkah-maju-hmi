<template>
  <div>
    <section class="hidden md:block">
      <nav
        class="
          container
          mx-auto
          lg:px-10
          md:flex
          justify-between
          py-5
          text-white
          font-normal
          text-lg
          subpixel-antialiased
          hidden
        "
      >
        <div>
          <nuxt-link to="/">
            <img
              src="~/assets/image/logo-komfaktek.png"
              alt="logo"
              class="h-10 w-auto"
            />
          </nuxt-link>
        </div>
        <div class="flex my-auto">
          <a href="reward.html" class="ml-8 hover:text-green-700 my-auto"
            >Reward</a
          >
          <a href="tulisan.html" class="ml-8 hover:text-green-700 my-auto"
            >Tulisan</a
          >
          <a href="galang.html" class="ml-8 hover:text-green-700 my-auto"
            >Galang Dana</a
          >
          <a href="gabung.html" class="ml-8 hover:text-green-700 my-auto"
            >Gabung HMI</a
          >
          <!-- jika login = false -->
          <nuxt-link
            to="/login"
            class="
              ml-8
              hover:bg-green-600
              bg-hijau-button
              py-1
              block
              px-8
              rounded-full
            "
            v-if="this.$auth.loggedIn == false"
            >Login</nuxt-link
          >
          <!-- jika login = true -->
          <nuxt-link
            to="/dashboard/profile"
            class="ml-8 hover:text-green-600 rounded-full flex"
            v-else
            ><div class="mr-4 my-auto">
              {{ this.$store.state.auth.user.name }}
            </div>
            <div v-if="this.$store.state.auth.user.user_detail.image">
              <img
                :src="this.$store.state.auth.user.user_detail.image"
                alt=""
                class="w-9 h-9 object-cover rounded-full"
              />
            </div>
            <div class="" v-else>
              <img
                src="~assets/image/profile-default.png"
                alt=""
                class="w-8 h-8 object-cover rounded-full"
              />
            </div>
          </nuxt-link>
        </div>
      </nav>
    </section>
  </div>
</template>
