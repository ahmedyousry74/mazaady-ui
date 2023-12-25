<template>
  <header class="w-full z-[999] bg-[#fafafa] overflow-hidden">
    <nav
      class="mx-auto flex sm:!px-[84px] px-[16px] sm:static lg:px-8 items-center justify-between py-3 h-[64px]"
      aria-label="Global"
    >
      <div class="flex justify-start items-center flex-row gap-[32px]">
        <div class="hidden lg:flex">
          <nuxt-link to="/">
            <img
              class="w-28 h-10 object-contain"
              src="/image/logo.svg"
              width="108"
              height="43"
              alt="Mazaady"
              loading="lazy"
            />
          </nuxt-link>
        </div>
        <div class="flex lg:hidden justify-center flex-row items-center gap-2">
          <nuxt-link
            to="/search"
            class="text-sm font-bold text-fourth-color mt-2"
          >
            <img src="/image/search.svg" />
          </nuxt-link>
          <nuxt-link
            to="/notifications"
            class="text-sm font-bold text-primary-color mt-2"
          >
            <img src="/image/notification.svg" />
          </nuxt-link>
          <div class="account__">
            <v-menu min-width="50px" rounded>
              <template v-slot:activator="{ props }">
                <span
                  class="font-bold"
                  style="letter-spacing: 0 !important"
                  v-bind="props"
                  variant="text"
                >
                  <img
                    src="/image/rectangle-12.png"
                    alt="profile"
                    width="30"
                    height="30"
                    class="rounded-full"
                  />
                </span>
              </template>
              <v-card>
                <v-card-text>
                  <div class="mx-auto text-center">
                    <nuxt-link to="/" variant="text" class="w-full">
                      Profile
                    </nuxt-link>
                    <v-divider class="my-2"></v-divider>
                    <v-btn variant="text" class="text-red w-full">
                      Logout
                    </v-btn>
                  </div>
                </v-card-text>
              </v-card>
            </v-menu>
          </div>
        </div>
        <PopoverGroup class="hidden lg:flex lg:gap-x-10 links">
          <nuxt-link
            to="/"
            class="text-sm font-bold leading-6 text-primary-color"
            >Home</nuxt-link
          >
          <nuxt-link
            to="/blogs"
            class="text-sm font-[400] leading-6 text-third-gray"
          >
            Blog
          </nuxt-link>
          <nuxt-link
            to="/gifts"
            class="text-sm font-[400] leading-6 text-third-gray"
          >
            Gifts
          </nuxt-link>
        </PopoverGroup>
      </div>

      <div class="hidden lg:flex lg:flex-1 lg:justify-end gap-[24px]">
        <nuxt-link
          to="/search"
          class="text-sm font-bold text-fourth-color mt-2"
        >
          <img src="/image/search.svg" />
        </nuxt-link>
        <hr class="h-auto w-[1px] bg-[#FFEAD2]" />
        <nuxt-link
          to="/notifications"
          class="text-sm font-bold text-primary-color mt-2"
        >
          <img src="/image/notification.svg" />
        </nuxt-link>
        <hr class="h-auto w-[1px] bg-[#FFEAD2]" />
        <div class="account__">
          <v-menu min-width="250px" rounded>
            <template v-slot:activator="{ props }">
              <span
                class="font-bold"
                style="letter-spacing: 0 !important"
                v-bind="props"
                variant="text"
              >
                <img
                  src="/image/rectangle-12.png"
                  alt="profile"
                  width="40"
                  height="40"
                  class="rounded-full"
                />
              </span>
            </template>
            <v-card>
              <v-card-text>
                <div class="mx-auto text-center">
                  <nuxt-link to="/" variant="text" class="w-full">
                    Profile
                  </nuxt-link>
                  <v-divider class="my-2"></v-divider>
                  <v-btn variant="text" class="text-red w-full"> Logout </v-btn>
                </div>
              </v-card-text>
            </v-card>
          </v-menu>
        </div>
        <div class="add__product">
          <v-btn
            variant="dense"
            class="text-white flex justify-center items-center flex-row gap-3 w-[172px] h-10 !rounded-[10px] px-4 pm-2"
          >
            <img src="/image/add-circle.svg" alt="add product" />
            <span class="mx-[4px]"> Add new product </span>
          </v-btn>
        </div>
        <button class="language flex justify-start items-center flex-row gap-1">
          <img src="/image/global.svg" alt="language" width="24" height="24" />
          <hr class="h-[16px] w-[1px] bg-[#E0E0E0]" />
          <span>EN</span>
        </button>
      </div>
      <div class="flex lg:hidden">
        <nuxt-link to="/">
          <img
            class="w-28 h-10 object-contain"
            src="/image/logo.svg"
            width="108"
            height="43"
            alt="Mazaady"
            loading="lazy"
          />
        </nuxt-link>
        <button
          type="button"
          class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-700"
          @click="mobileMenuOpen = true"
        >
          <span class="sr-only">Open main menu</span>
          <v-icon> mdi-menu </v-icon>
        </button>
      </div>
    </nav>
    <Dialog
      as="div"
      class="lg:hidden"
      @close="mobileMenuOpen = false"
      :open="mobileMenuOpen"
    >
      <div class="fixed inset-0 z-10" />
      <DialogPanel
        class="z-50 fixed inset-y-0 right-0 w-full overflow-y-auto bg-[#fcfcfc] px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-gray-900/10"
      >
        <div class="flex items-center justify-between">
          <a href="#">
            <img
              class="w-40 h-16 object-contain"
              src="/image/logo.svg"
              alt="depo"
              loading="lazy"
            />
          </a>
          <button
            type="button"
            class="-m-2.5 rounded-md p-2.5 text-gray-700"
            @click="mobileMenuOpen = false"
          >
            <span class="sr-only">Close menu</span>
            <v-icon> mdi-close </v-icon>
          </button>
        </div>
        <div class="mt-6 flow-root">
          <div class="-my-6 divide-y divide-gray-500/10">
            <div class="space-y-2 py-6 flex flex-col gap-3">
              <nuxt-link
                to="/"
                class="text-sm font-bold leading-6 text-primary-color"
                >Home</nuxt-link
              >
              <nuxt-link
                to="/blogs"
                class="text-sm font-[400] leading-6 text-third-gray"
              >
                Blog
              </nuxt-link>
              <nuxt-link
                to="/gifts"
                class="text-sm font-[400] leading-6 text-third-gray"
              >
                Gifts
              </nuxt-link>
            </div>
            <div class="add__product">
              <v-btn
                variant="dense"
                class="text-white flex justify-center items-center flex-row gap-3 w-[172px] h-10 !rounded-[10px] px-4 pm-2"
              >
                <img src="/image/add-circle.svg" alt="add product" />
                <span class="mx-[4px]"> Add new product </span>
              </v-btn>
            </div>
            <button
              class="language flex justify-start items-center flex-row gap-1 mt-3"
            >
              <img
                src="/image/global.svg"
                alt="language"
                width="24"
                height="24"
              />
              <hr class="h-[16px] w-[1px] bg-[#E0E0E0]" />
              <span>EN</span>
            </button>
          </div>
        </div>
      </DialogPanel>
    </Dialog>
  </header>
</template>

<script setup>
import { ref, onMounted, computed, watch } from "vue";

const mobileMenuOpen = ref(false);
</script>

<style scoped lang="scss">
.links {
  a {
    position: relative;
    &:after {
      border-radius: 999px;
      content: " ";
      position: absolute;
      left: 50%;
      bottom: 1px;
      transform: translateX(-50%) scaleX(0);
      transform-origin: 50% 50%;
      width: 80%;
      height: 5px;
      background-color: #d20653;
      transition: 0.4s ease-in-out;
      top: 41px;
    }
    &:hover::after {
      transform: translateX(-50%) scaleX(1);
    }
    &:hover {
      color: #d20653 !important;
    }
  }
  .router-link-active {
    color: #d20653 !important;
    &:after {
      transform: translateX(-50%) scaleX(1);
    }
  }
}
.add__product {
  button {
    background: linear-gradient(to right, #d20653, #ff951d);
  }
}
</style>
