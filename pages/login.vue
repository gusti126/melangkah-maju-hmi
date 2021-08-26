<template>
  <div>
    <div class="conatiner px-2 md:px-10 py-6">
      <div>
        <div class="bg-white rounded-xl p-4 md:w-3/6 md:mx-auto">
          <div>
            <img src="~/assets/image/logo-komfaktek.png" alt="" class="w-48" />
          </div>
          <div class="text-4xl font-bold text-hijau-button mt-4">Login</div>
          <div class="md:w-96 mx-auto mt-6">
            <div>
              <label for="email" class="text-xl">Email</label>
            </div>
            <div class="w-full mt-2">
              <input
                type="text"
                v-model="login.email"
                class="
                  rounded-full
                  p-2
                  w-full
                  focus:ring-2 focus:ring-hijau-button focus:text-hijau-button
                  border border-gray-500
                  focus:border-transparent focus:outline-none
                "
                placeholder="Email Address"
              />
            </div>
            <div class="mt-4">
              <label for="password" class="text-xl">Password</label>
            </div>
            <div class="w-full mt-2">
              <input
                type="password"
                v-model="login.password"
                class="
                  rounded-full
                  p-2
                  w-full
                  focus:ring-2 focus:ring-hijau-button focus:text-hijau-button
                  border border-gray-500
                  focus:border-transparent focus:outline-none
                "
                @keyup.enter="userLogin"
                placeholder="Input Password"
              />
            </div>
            <div class="w-full mt-4 text-right">
              <a href="" class="text-hijau-button">Lupa Password ?</a>
            </div>
            <div class="w-full mt-4">
              <div
                class="
                  bg-hijau-button
                  py-2
                  block
                  text-center text-white
                  rounded-full
                  hover:bg-hijau-header
                  cursor-pointer
                "
                @click="userLogin"
              >
                Login
              </div>
            </div>
            <div class="w-full mt-4">
              <nuxt-link
                to="register"
                class="
                  border border-hijau-button
                  py-2
                  block
                  text-center text-hijau-button
                  rounded-full
                  hover:bg-hijau-header
                "
                >Register</nuxt-link
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      login: {
        email: '',
        password: '',
      },
    }
  },
  methods: {
    async userLogin() {
      let response = await this.$auth
        .loginWith('local', { data: this.login })
        .then((ress) => {
          console.log(ress)
        })
    },
  },
}
</script>
