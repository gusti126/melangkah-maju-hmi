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
        <div class="">
          <a href="reward.html" class="ml-8 hover:text-green-700">Reward</a>
          <a href="tulisan.html" class="ml-8 hover:text-green-700">Tulisan</a>
          <a href="galang.html" class="ml-8 hover:text-green-700"
            >Galang Dana</a
          >
          <a href="gabung.html" class="ml-8 hover:text-green-700">Gabung HMI</a>
          <nuxt-link
            to="/login"
            class="
              ml-8
              hover:bg-green-600
              bg-hijau-button
              py-2
              px-8
              rounded-full
            "
            >Login</nuxt-link
          >
        </div>
      </nav>
    </section>
  </div>
</template>
