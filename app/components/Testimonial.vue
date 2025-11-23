<template>
  <section class="container mx-auto py-8 lg:py-16">
    <div class="flex justify-between">
      <div>
        <h2
          class="font-semibold text-[32px] uppercase bg-gradient-to-l from-[#00bdff] to-[#13447e] bg-clip-text text-transparent mb-6"
        >
          What Our Students Say
        </h2>

        <button
          class="flex justify-center items-center px-5 py-3 gap-2 bg-[#EFFAFF] border border-[#b9e7fb] rounded-full mb-8"
        >
          Review us on <img src="/icons/google.svg" />
        </button>
      </div>
      <div class="flex items-center gap-1">
        <button
          @click="prev"
          class="flex justify-center items-center size-10 border-2 border-[#00BDFF] rounded-full text-[#00BDFF] hover:text-white hover:bg-[#00BDFF] transition-all duration-200"
        >
          <ChevronLeft class="w-6 h-6 group-hover:text-white relative z-20" />
        </button>
        <button
          @click="next"
          class="flex justify-center items-center size-10 border-2 border-[#00BDFF] rounded-full text-[#00BDFF] hover:text-white hover:bg-[#00BDFF] transition-all duration-200"
        >
          <ChevronRight class="w-6 h-6 group-hover:text-white relative z-20" />
        </button>
      </div>
    </div>

    <!-- Slider -->
    <div class="relative overflow-hidden">
      <div
        class="flex transition-transform duration-500"
        :style="{
          transform: `translateX(-${currentIndex * (100 / itemsToShow)}%)`,
        }"
      >
        <div
          v-for="(testimonial, index) in testimonials"
          :key="index"
          class="flex-shrink-0 w-[33.3333%] px-2"
        >
          <div class="bg-[#F7F7F7] p-6 py-8 rounded-3xl">
            <div class="flex justify-between">
              <div class="flex items-center gap-2">
                <img :src="testimonial.image" alt="" />
                <div>
                  <h3 class="font-semibold text-[24px]">
                    {{ testimonial.name }}
                  </h3>
                  <p class="text-[16px]">{{ testimonial.university }}</p>
                </div>
              </div>
              <img src="/icons/google.svg" alt="" class="size-10" />
            </div>
            <div class="flex gap-1 mt-5">
              <Star
                v-for="i in 5"
                :key="i"
                class="fill-yellow-500 stroke-yellow-500"
              />
            </div>
            <p class="mt-2 text-gray-500">{{ testimonial.message }}</p>
          </div>
        </div>
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

const testimonials = ref([
  {
    image: "/images/avatar/5.png",
    name: "Guy Hawkins",
    university: "University Name",
    message:
      "Thanks to SEG, my dream of studying abroad came true. Their guidance made the whole process smooth and stress-free. I’m now studying at University of Manilla, Australia, and couldn’t be happier!",
  },
  {
    image: "/images/avatar/6.png",
    name: "Guy Hawkins",
    university: "University Name",
    message:
      "Thanks to SEG, my dream of studying abroad came true. Their guidance made the whole process smooth and stress-free. I’m now studying at University of Manilla, Australia, and couldn’t be happier!",
  },
  {
    image: "/images/avatar/7.png",
    name: "Guy Hawkins",
    university: "University Name",
    message:
      "Thanks to SEG, my dream of studying abroad came true. Their guidance made the whole process smooth and stress-free. I’m now studying at University of Manilla, Australia, and couldn’t be happier!",
  },
  {
    image: "/images/avatar/5.png",
    name: "Guy Hawkins",
    university: "University Name",
    message:
      "Thanks to SEG, my dream of studying abroad came true. Their guidance made the whole process smooth and stress-free. I’m now studying at University of Manilla, Australia, and couldn’t be happier!",
  },
  {
    image: "/images/avatar/6.png",
    name: "Guy Hawkins",
    university: "University Name",
    message:
      "Thanks to SEG, my dream of studying abroad came true. Their guidance made the whole process smooth and stress-free. I’m now studying at University of Manilla, Australia, and couldn’t be happier!",
  },
  {
    image: "/images/avatar/7.png",
    name: "Guy Hawkins",
    university: "University Name",
    message:
      "Thanks to SEG, my dream of studying abroad came true. Their guidance made the whole process smooth and stress-free. I’m now studying at University of Manilla, Australia, and couldn’t be happier!",
  },
  {
    image: "/images/avatar/5.png",
    name: "Guy Hawkins",
    university: "University Name",
    message:
      "Thanks to SEG, my dream of studying abroad came true. Their guidance made the whole process smooth and stress-free. I’m now studying at University of Manilla, Australia, and couldn’t be happier!",
  },
  {
    image: "/images/avatar/6.png",
    name: "Guy Hawkins",
    university: "University Name",
    message:
      "Thanks to SEG, my dream of studying abroad came true. Their guidance made the whole process smooth and stress-free. I’m now studying at University of Manilla, Australia, and couldn’t be happier!",
  },
  {
    image: "/images/avatar/7.png",
    name: "Guy Hawkins",
    university: "University Name",
    message:
      "Thanks to SEG, my dream of studying abroad came true. Their guidance made the whole process smooth and stress-free. I’m now studying at University of Manilla, Australia, and couldn’t be happier!",
  },
]);

const itemsToShow = 3;

const currentIndex = ref(0);

const maxIndex = testimonials.value.length - itemsToShow;

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
</script>
