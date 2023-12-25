<template>
  <div
    class="products bg-[#fff] rounded-[21px] p-6 flex justify-start items-start flex-col gap-6"
  >
    <div class="flex justify-between flex-row items-center w-full flex-wrap">
      <v-tabs
        v-model="model"
        centered
        class="tabs__btns flex justify-start items-start gap-2 flex-wrap"
      >
        <v-tab value="products" class="p-0"> Products </v-tab>
        <v-tab value="articles" class="p-0"> Articles </v-tab>
        <v-tab value="reviews" class="p-0"> Reviews </v-tab>
      </v-tabs>
      <div
        class="add__review sm:!relative sm:!top-0 sm:!right-0 fixed top-[80px] right-8 z-50"
      >
        <v-btn
          variant="dense"
          class="text-white flex justify-center items-center flex-row gap-3 w-[125px] h-10 !rounded-[10px] px-4 pm-2"
        >
          <img src="/image/add-circle.svg" alt="add product" />
          <span class="mx-[4px]"> Review </span>
        </v-btn>
      </div>
    </div>
    <div class="w-full">
      <v-window v-model="model" class="w-full">
        <v-window-item value="products" class="w-full">
          <h2
            class="font-[800] sm:!text-[32px] text-[24px] text-primary-gray mb-4"
          >
            Products
            <sup class="font-normal text-sm text-third-gray"> ( 12 ) </sup>
          </h2>
          <div class="flex justify-start flex-col items-start gap-8">
            <div class="w-full relative">
              <div class="flex justify-between items-start flex-row w-full">
                <div
                  class="flex justify-start items-start flex-row gap-4 flex-wrap"
                >
                  <div class="product__img relative">
                    <img
                      src="/image/rectangle-13.png"
                      alt="product"
                      width="145"
                      height="127"
                    />
                    <span
                      class="bg-primary-color text-[#fff] rounded-tl-full rounded-br-full px-5 py-2 absolute right-[0] top-[95px] text-xs"
                    >
                      Live auction
                    </span>
                  </div>
                  <div
                    class="product__desc flex justify-start items-start flex-col sm:!gap-4 gap-1"
                  >
                    <h1
                      class="text-primary-gray font-normal sm:!text-[18px] text-[12px] leading-6"
                    >
                      Six-piece clothing set (blouse - pants - hat and ...
                    </h1>
                    <p
                      class="text-third-gray font-bold sm:!text-[18px] text-[12px] leading-6"
                    >
                      starting price
                      <span
                        class="text-primary-gray font-bold sm:!text-[24px] text-[16px] leading-6"
                        >1000 EGP</span
                      >
                    </p>
                    <div
                      class="flex justify-start items-center flex-row gap-2 flex-wrap"
                    >
                      <span
                        class="text-third-gray font-normal sm:!text-[18px] text-[12px] leading-6"
                        >Lot starts in</span
                      >
                      <div
                        class="flex justify-start items-center flex-row gap-2 flex-wrap"
                      >
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                          ><span class="font-bold mx-1 text-lg"> 2 </span> days
                        </span>
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                        >
                          <span class="font-bold mx-1 text-lg"> 10 </span> Hours
                        </span>
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                        >
                          <span class="font-bold mx-1 text-lg"> 50 </span>
                          Minutes
                        </span>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="product__fav">
                  <button><img src="/image/vuesax.svg" alt="" /></button>
                </div>
              </div>
            </div>
            <div class="w-full relative">
              <div class="flex justify-between items-start flex-row w-full">
                <div
                  class="flex justify-start items-start flex-row gap-4 flex-wrap"
                >
                  <div class="product__img relative">
                    <img
                      src="/image/rectangle-13.png"
                      alt="product"
                      width="145"
                      height="127"
                    />
                    <span
                      class="bg-primary-orange text-[#fff] rounded-tl-full rounded-br-full px-5 py-2 absolute right-[0] top-[95px] text-xs"
                    >
                      Hot sale
                    </span>
                  </div>
                  <div
                    class="product__desc flex justify-start items-start flex-col sm:!gap-4 gap-1"
                  >
                    <h1
                      class="text-primary-gray font-normal sm:!text-[18px] text-[12px] leading-6"
                    >
                      Six-piece clothing set (blouse - pants - hat and ...
                    </h1>
                    <p
                      class="text-third-gray font-bold sm:!text-[18px] text-[12px] leading-6"
                    >
                      starting price
                      <span
                        class="text-primary-gray font-bold sm:!text-[24px] text-[16px] leading-6"
                        >1000 EGP</span
                      >
                    </p>
                    <div
                      class="flex justify-start items-center flex-row gap-2 flex-wrap"
                    >
                      <span
                        class="text-third-gray font-normal sm:!text-[18px] text-[12px] leading-6"
                        >Lot starts in</span
                      >
                      <div
                        class="flex justify-start items-center flex-row gap-2 flex-wrap"
                      >
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                          ><span class="font-bold mx-1 text-lg"> 2 </span> days
                        </span>
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                        >
                          <span class="font-bold mx-1 text-lg"> 10 </span> Hours
                        </span>
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                        >
                          <span class="font-bold mx-1 text-lg"> 50 </span>
                          Minutes
                        </span>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="product__fav">
                  <button><img src="/image/vuesax1.svg" alt="" /></button>
                </div>
              </div>
            </div>
            <div class="w-full relative">
              <div class="flex justify-between items-start flex-row w-full">
                <div
                  class="flex justify-start items-start flex-row gap-4 flex-wrap"
                >
                  <div class="product__img relative">
                    <img
                      src="/image/rectangle-13.png"
                      alt="product"
                      width="145"
                      height="127"
                    />
                    <span
                      class="bg-primary-color text-[#fff] rounded-tl-full rounded-br-full px-5 py-2 absolute right-[0] top-[95px] text-xs"
                    >
                      Live auction
                    </span>
                  </div>
                  <div
                    class="product__desc flex justify-start items-start flex-col sm:!gap-4 gap-1"
                  >
                    <h1
                      class="text-primary-gray font-normal sm:!text-[18px] text-[12px] leading-6"
                    >
                      Six-piece clothing set (blouse - pants - hat and ...
                    </h1>
                    <p
                      class="text-third-gray font-bold sm:!text-[18px] text-[12px] leading-6"
                    >
                      starting price
                      <span
                        class="text-primary-gray font-bold sm:!text-[24px] text-[16px] leading-6"
                        >1000 EGP</span
                      >
                    </p>
                    <div
                      class="flex justify-start items-center flex-row gap-2 flex-wrap"
                    >
                      <span
                        class="text-third-gray font-normal sm:!text-[18px] text-[12px] leading-6"
                        >Lot starts in</span
                      >
                      <div
                        class="flex justify-start items-center flex-row gap-2 flex-wrap"
                      >
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                          ><span class="font-bold mx-1 text-lg"> 2 </span> days
                        </span>
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                        >
                          <span class="font-bold mx-1 text-lg"> 10 </span> Hours
                        </span>
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                        >
                          <span class="font-bold mx-1 text-lg"> 50 </span>
                          Minutes
                        </span>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="product__fav">
                  <button><img src="/image/vuesax.svg" alt="" /></button>
                </div>
              </div>
            </div>
            <div class="w-full relative">
              <div class="flex justify-between items-start flex-row w-full">
                <div
                  class="flex justify-start items-start flex-row gap-4 flex-wrap"
                >
                  <div class="product__img relative">
                    <img
                      src="/image/rectangle-13.png"
                      alt="product"
                      width="145"
                      height="127"
                    />
                    <span
                      class="bg-primary-orange text-[#fff] rounded-tl-full rounded-br-full px-5 py-2 absolute right-[0] top-[95px] text-xs"
                    >
                      Hot sale
                    </span>
                  </div>
                  <div
                    class="product__desc flex justify-start items-start flex-col sm:!gap-4 gap-1"
                  >
                    <h1
                      class="text-primary-gray font-normal sm:!text-[18px] text-[12px] leading-6"
                    >
                      Six-piece clothing set (blouse - pants - hat and ...
                    </h1>
                    <p
                      class="text-third-gray font-bold sm:!text-[18px] text-[12px] leading-6"
                    >
                      starting price
                      <span
                        class="text-primary-gray font-bold sm:!text-[24px] text-[16px] leading-6"
                        >1000 EGP</span
                      >
                    </p>
                    <div
                      class="flex justify-start items-center flex-row gap-2 flex-wrap"
                    >
                      <span
                        class="text-third-gray font-normal sm:!text-[18px] text-[12px] leading-6"
                        >Lot starts in</span
                      >
                      <div
                        class="flex justify-start items-center flex-row gap-2 flex-wrap"
                      >
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                          ><span class="font-bold mx-1 text-lg"> 2 </span> days
                        </span>
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                        >
                          <span class="font-bold mx-1 text-lg"> 10 </span> Hours
                        </span>
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                        >
                          <span class="font-bold mx-1 text-lg"> 50 </span>
                          Minutes
                        </span>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="product__fav">
                  <button><img src="/image/vuesax1.svg" alt="" /></button>
                </div>
              </div>
            </div>
            <div class="w-full relative">
              <div class="flex justify-between items-start flex-row w-full">
                <div
                  class="flex justify-start items-start flex-row gap-4 flex-wrap"
                >
                  <div class="product__img relative">
                    <img
                      src="/image/rectangle-13.png"
                      alt="product"
                      width="145"
                      height="127"
                    />
                    <span
                      class="bg-primary-orange text-[#fff] rounded-tl-full rounded-br-full px-5 py-2 absolute right-[0] top-[95px] text-xs"
                    >
                      Hot sale
                    </span>
                  </div>
                  <div
                    class="product__desc flex justify-start items-start flex-col sm:!gap-4 gap-1"
                  >
                    <h1
                      class="text-primary-gray font-normal sm:!text-[18px] text-[12px] leading-6"
                    >
                      Six-piece clothing set (blouse - pants - hat and ...
                    </h1>
                    <p
                      class="text-third-gray font-bold sm:!text-[18px] text-[12px] leading-6"
                    >
                      starting price
                      <span
                        class="text-primary-gray font-bold sm:!text-[24px] text-[16px] leading-6"
                        >1000 EGP</span
                      >
                    </p>
                    <div
                      class="flex justify-start items-center flex-row gap-2 flex-wrap"
                    >
                      <span
                        class="text-third-gray font-normal sm:!text-[18px] text-[12px] leading-6"
                        >Lot starts in</span
                      >
                      <div
                        class="flex justify-start items-center flex-row gap-2 flex-wrap"
                      >
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                          ><span class="font-bold mx-1 text-lg"> 2 </span> days
                        </span>
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                        >
                          <span class="font-bold mx-1 text-lg"> 10 </span> Hours
                        </span>
                        <span
                          class="bg-second-orange text-primary-orange sm:!px-4 sm:!py-2 px-2 py-1 rounded-[24px] flex justify-center text-sm"
                        >
                          <span class="font-bold mx-1 text-lg"> 50 </span>
                          Minutes
                        </span>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="product__fav">
                  <button><img src="/image/vuesax1.svg" alt="" /></button>
                </div>
              </div>
            </div>
          </div>
        </v-window-item>
        <v-window-item value="articles">
          <div>
            articles
          </div>
        </v-window-item>
        <v-window-item value="reviews">
          <div>
            reviews
          </div>
        </v-window-item>
      </v-window>
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted, computed, watch } from "vue";
const model = ref("products");
</script>

<style lang="scss" scoped>
.add__review {
  button {
    background: linear-gradient(to right, #d20653, #ff951d);
  }
}
.product__fav{

  @media (max-width: 580px) {
    position: absolute;
    top: 10px;
    left: 7px;
    background: #fff;
    height: 24px;
    padding: 1px;
    border-radius: 50%;
  }
}
</style>
