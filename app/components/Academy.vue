<template>
  <section class="container mx-auto py-8 lg:py-16">
    <div class="max-w-4xl mx-auto">
      <h2
        class="font-['Cabin_Sketch'] font-bold text-4xl lg:text-6xl uppercase bg-gradient-to-l from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)] bg-clip-text text-transparent text-center"
      >
        Academic Excellence Meets Cultural Discovery
      </h2>
    </div>
    <div class="flex items-center gap-1"></div>

    <div class="relative overflow-hidden mt-10">
      <div
        class="flex transition-transform duration-500"
        :style="{
          transform: `translateX(-${currentIndex * (100 / itemsToShow)}%)`,
        }"
      >
        <div
          v-for="(academy, index) in academies"
          :key="index"
          class="flex-shrink-0 w-[33.3333%] px-1"
        >
          <img
            :src="academy.image"
            alt=""
            class="w-full aspect-square object-cover"
          />
        </div>
      </div>
      <div
        class="max-w-2xl absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-white/50 backdrop-blur-xl p-10 rounded-2xl z-10"
      >
        <h2 class="text-2xl font-bold text-center">
          {{ selectedAcademy.name }}
        </h2>
        <p class="text-center">{{ selectedAcademy.message }}</p>
        <button
          @click="prev"
          class="absolute top-1/2 left-0 transform -translate-y-1/2 -translate-x-1/2 z-20 bg-white/50 backdrop-blur-xl size-9 rounded-full flex justify-center items-center"
        >
          <ChevronLeft class="size-7 group-hover:text-white relative z-20" />
        </button>
        <button
          @click="next"
          class="absolute top-1/2 right-0 transform -translate-y-1/2 translate-x-1/2 z-20 bg-white/50 backdrop-blur-xl size-9 rounded-full flex justify-center items-center"
        >
          <ChevronRight class="size-7 group-hover:text-white relative z-20" />
        </button>
      </div>
    </div>

    <div class="flex justify-center mt-10">
      <button
        class="py-4 px-8 rounded-lg bg-gradient-to-r from-[#13447e] to-[#00bdff] border-none font-['Cabin_Sketch'] font-normal text-xl text-white transition-opacity duration-200 hover:opacity-90"
      >
        Apply Now
      </button>
    </div>
  </section>
</template>

<script setup>
import { ChevronLeft, ChevronRight, Star } from "lucide-vue-next";
import { ref } from "vue";

const academies = ref([
  {
    image: "/images/academy/1.png",
    name: "Elite University Visits",
    message:
      "Tour Harvard, MIT, Stanford, Oxford, and other world-leading institutions with exclusive campus access, library tours, and student interactions",
  },
  {
    image: "/images/academy/2.png",
    name: "Elite University Visits 2",
    message:
      "Tour Harvard, MIT, Stanford, Oxford, and other world-leading institutions with exclusive campus access, library tours, and student interactions",
  },
  {
    image: "/images/academy/3.png",
    name: "Elite University Visits 3",
    message:
      "Tour Harvard, MIT, Stanford, Oxford, and other world-leading institutions with exclusive campus access, library tours, and student interactions",
  },
  {
    image: "/images/academy/1.png",
    name: "Elite University Visits",
    message:
      "Tour Harvard, MIT, Stanford, Oxford, and other world-leading institutions with exclusive campus access, library tours, and student interactions",
  },
  {
    image: "/images/academy/2.png",
    name: "Elite University Visits 2",
    message:
      "Tour Harvard, MIT, Stanford, Oxford, and other world-leading institutions with exclusive campus access, library tours, and student interactions",
  },
  {
    image: "/images/academy/3.png",
    name: "Elite University Visits 3",
    message:
      "Tour Harvard, MIT, Stanford, Oxford, and other world-leading institutions with exclusive campus access, library tours, and student interactions",
  },
  {
    image: "/images/academy/1.png",
    name: "Elite University Visits",
    message:
      "Tour Harvard, MIT, Stanford, Oxford, and other world-leading institutions with exclusive campus access, library tours, and student interactions",
  },
  {
    image: "/images/academy/2.png",
    name: "Elite University Visits 2",
    message:
      "Tour Harvard, MIT, Stanford, Oxford, and other world-leading institutions with exclusive campus access, library tours, and student interactions",
  },
  {
    image: "/images/academy/3.png",
    name: "Elite University Visits 3",
    message:
      "Tour Harvard, MIT, Stanford, Oxford, and other world-leading institutions with exclusive campus access, library tours, and student interactions",
  },
]);

const itemsToShow = 3;

const currentIndex = ref(0);

const maxIndex = academies.value.length - itemsToShow;

function next() {
  if (currentIndex.value < maxIndex) {
    currentIndex.value++;
  }
}

function prev() {
  if (currentIndex.value > 0) {
    currentIndex.value--;
  }
}

const selectedAcademy = computed(() => {
  return academies.value[currentIndex.value];
});
</script>
