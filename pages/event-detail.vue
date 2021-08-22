<template>
  <div>
    <navmobile />
    <div
      class="
        bg-center bg-cover
        sm:bg-left-top
        lg:bg-center
        bg-hijau-header
        rounded-b-3xl
        h-52
        hidden
        md:block
      "
    >
      <navbar />
    </div>
    <div class="grid grid-flow-row grid-cols-12 gap-4 md:px-10 px-2 md:-mt-32">
      <div class="col-span-12 md:col-span-8">
        <div class="bg-white rounded-lg p-6">
          <div>
            <img
              src="https://lorempixel.com/400/200/technics/"
              alt=""
              class="w-full rounded-lg"
            />
          </div>
          <div class="text-2xl font-semibold text-gray-700 mt-4">
            Java Programming Master Class For Software
          </div>
          <div class="mt-2 text-gray-700 leading-7">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque cum
            culpa dicta laudantium porro quisquam corporis blanditiis enim aut,
            autem consectetur ratione unde est rem tempore tempora molestias
            deserunt modi, ex ipsum? Harum inventore sunt ex aut consequuntur
            nostrum enim beatae provident sequi esse sint quos illum ipsum
            quaerat cupiditate vitae deserunt labore, in totam, fugiat
            voluptate? In aliquid beatae aspernatur quas doloremque dolor, aut
            dicta voluptas. Exercitationem at voluptatum eligendi expedita
            consectetur ex unde cumque praesentium laudantium est vel ducimus
            fuga, eveniet autem quas dolor similique necessitatibus aperiam
            quaerat asperiores repellendus! Sint ab minus, dolorem omnis odio
            nisi quis.
          </div>
        </div>
        <div class="mt-4 bg-white rounded-lg p-6">
          <div class="text-gray-700 text-lg font-semibold mb-4">Pemateri</div>
          <div class="flex text-center justify-around">
            <div>
              <img
                src="https://images.unsplash.com/photo-1628094591334-708f2982a850?ixid=MnwxMjA3fDB8MHx0b3BpYy1mZWVkfDcyfHRvd0paRnNrcEdnfHxlbnwwfHx8fA%3D%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=60"
                alt=""
                class="
                  rounded-full
                  w-28
                  h-28
                  object-cover
                  p-2
                  border-hijau-header border-2
                  mx-auto
                "
              />
              <div class="mt-2 text-gray-700 font-medium">Steven Wiliams</div>
              <div class="text-gray-600 text-sm">Manager Engineer Tesla</div>
            </div>
            <div>
              <img
                src="https://images.unsplash.com/photo-1619358494796-212138ae5df3?ixid=MnwxMjA3fDB8MHx0b3BpYy1mZWVkfDUzfHRvd0paRnNrcEdnfHxlbnwwfHx8fA%3D%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=60"
                alt=""
                class="
                  rounded-full
                  w-28
                  h-28
                  object-cover
                  p-2
                  border-hijau-header border-2
                  mx-auto
                "
              />
              <div class="mt-2 text-gray-700 font-medium">Julian Nafitulun</div>
              <div class="text-gray-600 text-sm">Product Manager Tesla</div>
            </div>
          </div>
        </div>
      </div>

      <div class="col-span-12 md:col-span-4">
        <div class="bg-white p-6 rounded-lg sticky top-4">
          <div class="text-gray-700 text-lg font-semibold mb-4">
            Pelaksanaan
          </div>
          <div>
            <div class="flex justify-between">
              <img
                src="~/assets/image/icon/whh_student.svg"
                alt=""
                class="w-7 mr-2"
              />
              07/08/21
            </div>
            <div class="flex justify-between my-6">
              <img
                src="~/assets/image/icon/emojione-v1-alarm-clock.svg"
                alt=""
                class="w-7 mr-2"
              />
              07/08/21
            </div>
            <div class="flex justify-between my-6">
              <img
                src="~/assets/image/icon/certificate.svg"
                alt=""
                class="w-7 mr-2"
              />
              Bersertifikat
            </div>
            <hr />
            <div class="my-6 flex">
              <img
                src="https://images.unsplash.com/photo-1627691541764-85b6e9003bec?ixid=MnwxMjA3fDB8MHx0b3BpYy1mZWVkfDc4fHRvd0paRnNrcEdnfHxlbnwwfHx8fA%3D%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=60"
                alt=""
                class="rounded-full object-cover w-14 h-14 mr-4"
              />
              <div class="my-auto">
                <div class="font-medium text-gray-700">Jeni Lamari</div>
                <div class="text-gray-700 text-sm">Moderator</div>
              </div>
            </div>
            <hr />
            <div class="mt-6">
              <div
                class="
                  bg-hijau-button
                  rounded-full
                  py-2
                  text-white text-center
                  hover:bg-hijau-header
                  cursor-pointer
                "
              >
                Daftar Event
              </div>
            </div>
            <!-- <div class="flex mt-6 justify-between">
              <div class="">
                <a href="">
                  <img
                    src="~/assets/image/icon/fa-solid_share.svg"
                    alt="Share"
                    class="w-6"
                  />
                </a>
              </div>
              <div class="">
                <a href="">
                  <img
                    src="~/assets/image/icon/logos_whatsapp.svg"
                    alt="Share"
                    class="w-6"
                  />
                </a>
              </div>
              <div class="">
                <a href="">
                  <img
                    src="~/assets/image/icon/bi_facebook.svg"
                    alt="Share"
                    class="w-6"
                  />
                </a>
              </div>
            </div> -->
          </div>
        </div>
      </div>
    </div>
    <div class="md:px-10 px2 mt-4">
      <div class="rounded-lg bg-white p-6">
        <div class="font-semibold text-lg text-gray-700">Event Lainnya</div>

        <div class="grid grid-flow-row grid-cols-12 gap-6 mt-6">
          <div
            class="col-span-12 md:col-span-3 p-4 rounded-lg border"
            v-for="p of 4"
          >
            <nuxt-link to="">
              <div>
                <img
                  src="https://lorempixel.com/200/200/technics/"
                  alt=""
                  class="rounded-lg w-full object-cover h-40"
                />
              </div>
              <div class="text-lg font-semibold text-gray-700 mt-2">
                Java Programming Master Class For Software
              </div>
              <div class="mt-4 flex justify-between">
                <div class="flex">
                  <div>
                    <img
                      src="~/assets/image/icon/emojione-v1-alarm-clock.svg"
                      alt=""
                      class="w-4 mr-2"
                    />
                  </div>
                  <div class="my-auto text-gray-700 text-xs">09/08/21</div>
                </div>
                <div class="flex">
                  <div>
                    <img
                      src="~/assets/image/icon/whh_student.svg"
                      alt=""
                      class="w-4 mr-2"
                    />
                  </div>
                  <div class="my-auto text-gray-700 text-xs">100 Peserta</div>
                </div>
              </div>
            </nuxt-link>
          </div>
        </div>
      </div>
    </div>
    <Cfooter />
  </div>
</template>
