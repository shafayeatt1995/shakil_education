<template>
  <section class="container mx-auto py-8 lg:py-16 lg:pt-24">
    <div class="flex flex-col lg:flex-row gap-10 lg:gap-5">
      <div class="flex-1 relative px-2 lg:px-0" data-aos="fade-right">
        <img
          src="/icons/plane.svg"
          alt=""
          class="absolute -top-14 right-1/4 size-14"
        />
        <h2
          class="font-['Cabin_Sketch'] font-bold text-4xl lg:text-7xl uppercase bg-gradient-to-r from-[#00bdff] to-[#13447e] bg-clip-text text-transparent text-center lg:text-left"
        >
          Why Travel with Shakil Education Group?
        </h2>
        <p class="text-gray-500 mt-5 text-center lg:text-left">
          we believe travel is more than just visiting new places—it’s about
          creating unforgettable experiences.
        </p>
        <div class="flex justify-center lg:justify-start mt-5 lg:mt-16">
          <button
            class="py-4 px-8 rounded-lg bg-gradient-to-r from-[#13447e] to-[#00bdff] border-none font-['Cabin_Sketch'] font-normal text-xl text-white transition-opacity duration-200 hover:opacity-90"
          >
            Book your tour today
          </button>
        </div>
      </div>
      <div class="flex-1" data-aos="fade-left">
        <img
          src="/images/hero/travel.png"
          alt=""
          class="size-full object-cover lg:rounded-2xl"
        />
      </div>
    </div>
    <div class="relative px-2 lg:px-0">
      <div
        class="grid grid-cols-1 lg:grid-cols-3 gap-10 lg:gap-16 mt-5 lg:mt-40"
      >
        <div
          v-for="(feature, i) in features"
          :key="i"
          data-aos="fade-up"
          :data-aos-delay="200 * i"
        >
          <h3 class="font-bold text-2xl md:text-xl lg:text-2xl text-[#13447E]">
            {{ feature.title }}
          </h3>
          <p class="font-normal text-base leading-[1.5em] text-[#000000]">
            {{ feature.description }}
          </p>
        </div>
      </div>
      <img
        src="/icons/bag.svg"
        alt=""
        class="hidden lg:inline-block absolute -top-[120%] left-[5%]"
      />
      <img
        src="/icons/camera.svg"
        alt=""
        class="hidden lg:inline-block absolute -top-[120%] right-[40%]"
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
