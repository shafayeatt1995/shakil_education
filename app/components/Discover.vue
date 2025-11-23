<template>
  <section class="container mx-auto px-2 lg:px-0">
    <div class="flex flex-col lg:flex-row gap-5 py-8 lg:py-16">
      <div class="w-full">
        <div class="flex flex-col gap-4">
          <h2
            class="font-['Cabin_Sketch'] font-bold text-3xl lg:text-5xl uppercase bg-gradient-to-l from-[#00bdff] to-[#13447e] bg-clip-text text-transparent"
          >
            Discover the world, one journey at a time.
          </h2>
          <p>
            From breathtaking landscapes to cultural wonders, we craft journeys
            that bring your dream destinations to life. Whether you're planning
            a relaxing getaway or an adventure-filled expedition, our team
            ensures every detail is taken care of.
          </p>
        </div>

        <div class="flex flex-col gap-2 mt-8">
          <div
            v-for="(feature, i) in features"
            :key="i"
            class="flex flex-row gap-2"
          >
            <div class="flex flex-row items-center gap-1">
              <p
                class="size-5 rounded-full flex justify-center items-center bg-[#FFABCC]"
              >
                <Check :size="14" />
              </p>
            </div>
            <span
              class="font-normal text-base leading-[1.5em] text-[#6B7280]"
              >{{ feature }}</span
            >
          </div>
        </div>
      </div>
      <div class="w-full">
        <iframe
          width="100%"
          src="https://www.youtube.com/embed/d9kgRkXeVTI?si=qeR8oFwYERJFhIOU"
          title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
          referrerpolicy="strict-origin-when-cross-origin"
          allowfullscreen
          class="rounded-2xl h-56 md:h-72 lg:h-96"
        ></iframe>
      </div>
    </div>
    <div class="py-8 lg:py-16">
      <div
        class="grid grid-cols-2 md:grid-cols-4 gap-x-[1px] gap-y-[1px] bg-gray-300"
      >
        <div
          class="flex items-center gap-4 lg:gap-10 bg-white justify-center font-['Cabin_Sketch']"
          v-for="(achievement, i) in achievements"
          :key="i"
        >
          <span
            class="font-bold text-3xl lg:text-6xl uppercase bg-gradient-to-l from-[#00bdff] to-[#13447e] bg-clip-text text-transparent"
            >{{ achievement.count }}</span
          >
          <span class="text-xl break-all">
            {{ achievement.message.split(" ")[0] }}
            <br />
            {{ achievement.message.split(" ")[1] }}
          </span>
        </div>
      </div>
      <div
        class="bg-[#13447E] rounded-3xl flex items-center justify-center relative mt-10 lg:mt-52"
      >
        <img
          src="/images/hero/flying.png"
          alt="Image"
          class="w-1/3 absolute -left-1 bottom-0 z-10 hidden lg:inline-block"
        />
        <p
          class="font-bold text-2xl lg:text-[32px] uppercase text-white px-4 lg:w-1/2 py-10 lg:py-20 relative z-20"
        >
          Your travel companion that carries all the information
        </p>
        <img
          src="/images/hero/happy.png"
          alt="Image"
          class="w-[22%] absolute right-0 bottom-0 z-10 hidden lg:inline-block"
        />
      </div>
    </div>
  </section>
</template>

<script setup>
import { Check } from "lucide-vue-next";

const features = ref([
  "Premium Stays & Exclusive Deals",
  "Tailored Packages for Every Traveler",
  "Unmatched Support Before & During Trips",
]);
const achievements = ref([
  {
    count: "12k+",
    message: "Happy travelers",
  },
  {
    count: "10k+",
    message: "Flights booked",
  },
  {
    count: "5k+",
    message: "Tours organized",
  },
  {
    count: "8k+",
    message: "Hotel stays",
  },
]);
</script>
