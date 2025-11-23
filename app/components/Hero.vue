<template>
  <section class="container mx-auto py-8 lg:py-16 px-2 lg:px-0">
    <div class="flex flex-col lg:flex-row items-center gap-10 lg:gap-5">
      <div class="w-full flex flex-col gap-5 px-4 lg:px-0 relative">
        <div class="absolute -top-3/4 right-0 z-[1] hidden lg:block">
          <img
            src="/icons/decorative-brush.svg"
            alt="Decorative"
            class="w-full h-full object-contain"
          />
        </div>
        <h1
          class="font-['Cabin_Sketch'] font-bold text-4xl lg:text-6xl uppercase bg-gradient-to-l from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)] bg-clip-text text-transparent"
        >
          Discover the world, one journey at a time.
        </h1>
        <p class="font-normal text-base md:text-xl text-gray-500">
          Handpicked travel packages designed to make every trip unforgettable.
        </p>
        <div>
          <button
            class="py-4 px-8 rounded-lg bg-gradient-to-r from-[#13447e] to-[#00bdff] border-none font-['Cabin_Sketch'] font-normal text-xl text-white transition-opacity duration-200 hover:opacity-90"
          >
            Book your tour today
          </button>
        </div>
      </div>
      <div class="w-full flex flex-col lg:flex-row items-center gap-7">
        <div class="flex gap-2 lg:flex-col">
          <img
            src="/images/hero/student.png"
            alt="Hero"
            class="lg:max-w-72 w-1/2 lg:w-auto aspect-square object-cover drop-shadow-[0px_2px_9px_rgba(30,161,219,0.6)] rounded-3xl"
          />
          <img
            src="/images/hero/nasa.png"
            alt="Hero"
            class="lg:max-w-72 w-1/2 lg:w-auto aspect-square object-cover drop-shadow-[0px_2px_9px_rgba(30,161,219,0.6)] rounded-3xl"
          />
        </div>
        <div class="flex-1 flex flex-col gap-6 relative">
          <div class="flex">
            <NuxtLink
              to="/"
              class="text-[#13447E] font-medium text-xl flex border-b-2 border-[#00BDFF]"
              >EXPLORE BEST PACKAGES <MoveUpRight
            /></NuxtLink>
          </div>
          <img
            src="/images/hero/tour-package-card.png"
            alt="Tour packages"
            class="w-full max-h-72 object-cover rounded-3xl"
          />
          <div class="grid grid-cols-2 mt-4">
            <div class="flex -space-x-5">
              <img
                v-for="(_, i) in 4"
                class="size-16 rounded-full inline-block"
                :src="`/images/avatar/${i + 1}.png`"
                alt="avatar"
              />
            </div>
            <div class="justify-self-center flex flex-col items-center">
              <p>4.6 Star Rated</p>
              <div class="flex gap-1">
                <Star
                  v-for="(_, i) in 4"
                  :key="i"
                  class="fill-yellow-500 stroke-yellow-500"
                />
                <StarHalf class="fill-yellow-500 stroke-yellow-500" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { MoveUpRight, Star, StarHalf } from "lucide-vue-next";
</script>
