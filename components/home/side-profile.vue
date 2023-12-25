<template>
  <div class="side_profile flex justify-start flex-col items-start gap-6">
    <div
      class="profile bg-[#fff] rounded-[21px] p-6 flex justify-start items-start flex-col gap-6"
    >
      <div class="profile__info flex justify-start items-start flex-col sm:!gap-4 gap-2">
        <img
          src="/image/rectangle-12.png"
          alt="profile"
          width="100"
          height="100px"
          class="rounded"
        />
        <h2 class="text-primary-gray font-bold sm:text-[24px] text-[18px] leading-6">
          Hala Ahmed
        </h2>
        <p class="text-second-gray font-normal text-[14px] leading-5">
          I am Hala Ahmed, I am the owner of the local brand called Beauty which
          is for Mackeup and Skin Care.
        </p>
      </div>
      <div class="profile__data flex justify-start flex-row items-center sm:!gap-4 gap-1 flex-wrap">
        <div
          class="flex justify-between flex-row items-center gap-[6px] px-2 py-3 bg-second-orange rounded-[18px]"
        >
          <div>
            <img src="/image/user-tick.svg" alt="user" width="24" height="24" />
          </div>
          <div class="flex justify-between flex-col items-start gap-[3px]">
            <span class="font-bold text-primary-gray text-sm">5</span>
            <span class="font-normal text-primary-orange text-xs"
              >Following</span
            >
          </div>
        </div>
        <div
          class="flex justify-between flex-row items-center gap-[6px] px-2 py-3 bg-second-orange rounded-[18px]"
        >
          <div>
            <img
              src="/image/profile-2user.svg"
              alt="user"
              width="24"
              height="24"
            />
          </div>
          <div class="flex justify-between flex-col items-start gap-[3px]">
            <span class="font-bold text-primary-gray text-sm">20</span>
            <span class="font-normal text-primary-orange text-xs"
              >Followers</span
            >
          </div>
        </div>
        <div
          class="flex justify-between flex-row items-center gap-[6px] px-2 py-3 bg-second-orange rounded-[18px]"
        >
          <div>
            <img
              src="/image/magic-star.svg"
              alt="user"
              width="24"
              height="24"
            />
          </div>
          <div class="flex justify-between flex-col items-start gap-[3px]">
            <span class="font-bold text-primary-gray text-sm"
              >4.2
              <span class="font-thin text-third-gray text-[10px]"> (14) </span>
            </span>
            <span class="font-normal text-primary-orange text-xs">Rate</span>
          </div>
        </div>
      </div>
      <div class="follow__btn w-full">
        <v-btn
          variant="dense"
          class="text-white flex justify-center items-center flex-row gap-3 w-full !h-12 !rounded-[14px] px-4 pm-2"
        >
          <span class="font-semibold text-[16px]"> follow </span>
        </v-btn>
      </div>
    </div>
    <homeQr />
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.follow__btn {
  button {
    background: linear-gradient(to right, #d20653, #ff951d);
}
}
.qr__bg{
    background: linear-gradient(to right, #d20653, #ff951d);
}
</style>
