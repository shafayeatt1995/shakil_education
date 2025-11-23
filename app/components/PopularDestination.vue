<template>
  <section class="container mx-auto py-8 lg:py-16 lg:pt-24">
    <div class="flex">
      <div class="flex-1 relative">
        <img
          src="/icons/plane.svg"
          alt=""
          class="absolute -top-14 right-1/4 size-14"
        />
        <h2
          class="font-['Cabin_Sketch'] font-bold text-7xl uppercase bg-gradient-to-r from-[#00bdff] to-[#13447e] bg-clip-text text-transparent"
        >
          Why Travel with Shakil Education Group?
        </h2>
        <p class="text-gray-500 mt-5">
          we believe travel is more than just visiting new places—it’s about
          creating unforgettable experiences.
        </p>
        <button
          class="py-4 px-8 rounded-lg bg-gradient-to-r from-[#13447e] to-[#00bdff] border-none font-['Cabin_Sketch'] font-normal text-xl text-white transition-opacity duration-200 hover:opacity-90 mt-16"
        >
          Book your tour today
        </button>
      </div>
      <div class="flex-1">
        <img
          src="/images/hero/travel.png"
          alt=""
          class="size-full object-cover rounded-2xl"
        />
      </div>
    </div>
    <div class="relative">
      <div class="grid grid-cols-3 gap-20 mt-40">
        <div class="" v-for="(feature, i) in features" :key="i">
          <h3 class="font-bold text-2xl md:text-xl lg:text-2xl text-[#13447E]">
            {{ feature.title }}
          </h3>
          <p class="font-normal text-base leading-[1.5em] text-[#000000]">
            {{ feature.description }}
          </p>
        </div>
      </div>
      <img src="/icons/bag.svg" alt="" class="absolute -top-[120%] left-[5%]" />
      <img
        src="/icons/camera.svg"
        alt=""
        class="absolute -top-[120%] right-[40%]"
      />
    </div>
  </section>
</template>

<script setup>
const features = ref([
  {
    title: "Trust",
    description:
      "Certified Tour Operator, Official Academic Partner, Reliable Travel Companion",
  },
  {
    title: "Expertise",
    description:
      "Expert Guides, Experienced Coordinators, Educational Itinerary, University Visits",
  },
  {
    title: "Value",
    description: "All-inclusive Packages, Transparent Pricing, Group Discounts",
  },
]);
</script>
