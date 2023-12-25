<template>
  <div class="qr__code w-full">
    <div
      class="qr__code bg-[#fff] rounded-[21px] p-6  justify-start items-start flex-col gap-6 !w-full hidden md:flex"
    >
      <div class="flex justify-between items-center flex-row w-full">
        <div>
          <h2 class="text-primary-gray font-bold text-[24px] leading-6">
            QR Code
          </h2>
        </div>
        <div class="flex justify-end items-center flex-row gap-6">
          <button>
            <img src="/image/eye.svg" alt="eye" width="24" height="24" />
          </button>
          <button>
            <img
              src="/image/document-download.svg"
              alt="download"
              width="24"
              height="24"
            />
          </button>
          <button>
            <img
              src="/image/send-square.svg"
              alt="send-square"
              width="24"
              height="24"
            />
          </button>
        </div>
      </div>
      <div
        class="bg-second-orange rounded-[18px] px-4 py-[17px] flex justify-start items-center flex-row w-full gap-2"
      >
        <img
          src="/image/document-download2.svg"
          alt="download"
          width="24"
          height="24"
        />
        <span class="text-primary-gray text-xs font-normal">
          Download the QR code or share it with your friends.
        </span>
      </div>
      <div class="qr__bg rounded-[20px] p-5 w-full">
        <div
          class="bg-[#fff] flex justify-center items-center flex-col gap-2 p-4"
        >
          <img
            class="w-[152px] h-[48px] object-contain"
            src="/image/logo.svg"
            width="152"
            height="48"
            alt="Mazaady"
            loading="lazy"
          />
          <h2 class="font-bold text-2xl text-primary-gray">Hala Ahmed</h2>
          <img
            class="w-[135px] h-[135px] object-contain"
            src="/image/World-Static.svg"
            width="135"
            height="135"
            alt="qr"
            loading="lazy"
          />
          <span class="font-normal text-sm text-primary-gray"
            >Follow Us on Mazaady</span
          >
        </div>
      </div>
    </div>
    <v-expansion-panels
      class="mb-6 bg-[#fff] rounded-[21px] p-6 justify-start items-start flex-col gap-6 w-full flex md:!hidden"
      
    >
      <v-expansion-panel>
        <v-expansion-panel-title expand-icon="mdi-menu-down">
          <div class="flex justify-between items-center flex-row w-full">
            <div>
              <h2 class="text-primary-gray font-bold sm:text-[24px] text-[18px] leading-6">
                QR Code
              </h2>
            </div>
            <div class="flex justify-end items-center flex-row gap-6">
              <button>
                <img src="/image/eye.svg" alt="eye" width="24" height="24" />
              </button>
              <button>
                <img
                  src="/image/document-download.svg"
                  alt="download"
                  width="24"
                  height="24"
                />
              </button>
              <button>
                <img
                  src="/image/send-square.svg"
                  alt="send-square"
                  width="24"
                  height="24"
                />
              </button>
            </div>
          </div>
        </v-expansion-panel-title>
        <v-expansion-panel-text>
          <div class="flex justify-start items-start flex-col gap-6 mt-4">
            <div
              class="bg-second-orange rounded-[18px] px-4 py-[17px] flex justify-start items-center flex-row w-full gap-2"
            >
              <img
                src="/image/document-download2.svg"
                alt="download"
                width="24"
                height="24"
              />
              <span class="text-primary-gray text-xs font-normal">
                Download the QR code or share it with your friends.
              </span>
            </div>
            <div class="qr__bg rounded-[20px] p-5 w-full">
              <div
                class="bg-[#fff] flex justify-center items-center flex-col gap-2 p-4"
              >
                <img
                  class="w-[152px] h-[48px] object-contain"
                  src="/image/logo.svg"
                  width="152"
                  height="48"
                  alt="Mazaady"
                  loading="lazy"
                />
                <h2 class="font-bold sm:text-[24px] text-[18px] text-primary-gray">Hala Ahmed</h2>
                <img
                  class="w-[135px] h-[135px] object-contain"
                  src="/image/World-Static.svg"
                  width="135"
                  height="135"
                  alt="qr"
                  loading="lazy"
                />
                <span class="font-normal text-sm text-primary-gray"
                  >Follow Us on Mazaady</span
                >
              </div>
            </div>
          </div>
        </v-expansion-panel-text>
      </v-expansion-panel>
    </v-expansion-panels>
  </div>
</template>

<script setup>
import {ref} from 'vue'
// const panel = ref[1]
</script>

<style lang="scss" scoped>
.qr__bg {
  background: linear-gradient(to right, #d20653, #ff951d);
}
</style>
