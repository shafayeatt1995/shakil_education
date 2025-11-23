<script setup>
import MasonryWall from "@yeger/vue-masonry-wall";

const images = [
  "/images/gallery/1.png",
  "/images/gallery/3.png",
  "/images/gallery/2.png",
  "/images/gallery/7.png",
  "/images/gallery/5.png",
  "/images/gallery/6.png",
  "/images/gallery/4.png",
];
</script>

<template>
  <!-- <section class="container mx-auto px-4 py-6">
    <MasonryWall :items="images" :column-width="300" :gap="8" :ssr-columns="1">
      <template #default="{ item }">
        <img :src="item" class="w-full block rounded-lg" alt="Gallery" />
      </template>
    </MasonryWall>

    <div class="grid grid-cols-4">
      <div class="col-span-3"></div>
      <div class="relative">
        <img
          src="/icons/gallery-plane.svg"
          alt=""
          class="absolute -z-[1] -top-[170%] right-5"
        />
        <h3 class="font-bold text-6xl text-[#13447E] text-center">Gallery</h3>
        <p class="text-gray-600 text-center mt-3">
          See exciting photos from our photo gallery &amp; choose your next trip
          easily
        </p>
      </div>
    </div>
  </section> -->

  <section class="container mx-auto px-4 py-6">
    <div class="grid grid-cols-4">
      <div>
        <img src="/images/gallery/1.png" alt="" class="w-full" />
        <img src="/images/gallery/2.png" alt="" class="w-full" />
      </div>
      <div>
        <img src="/images/gallery/3.png" alt="" class="w-full" />
        <img src="/images/gallery/4.png" alt="" class="w-full" />
      </div>
      <div>
        <img src="/images/gallery/5.png" alt="" class="w-full" />
        <img src="/images/gallery/6.png" alt="" class="w-full" />
      </div>
      <div>
        <img src="/images/gallery/7.png" alt="" class="w-full" />
        <div class="relative">
          <img
            src="/icons/gallery-plane.svg"
            alt=""
            class="absolute -z-[1] -top-[170%] right-5"
          />
          <h3 class="font-bold text-6xl text-[#13447E] text-center">Gallery</h3>
          <p class="text-gray-600 text-center mt-3">
            See exciting photos from our photo gallery &amp; choose your next
            trip easily
          </p>
        </div>
      </div>
    </div>
  </section>
</template>
