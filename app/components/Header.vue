<template>
  <section class="shadow-md w-full">
    <div class="container mx-auto">
      <nav class="w-full bg-white py-5 px-2 lg:px-0">
        <div class="flex items-center justify-between gap-5">
          <NuxtLink to="/" class="max-w-24 lg:max-w-36 max-h-11">
            <img
              src="/images/logo.png"
              alt="Logo"
              class="w-full h-full object-contain"
            />
          </NuxtLink>

          <div
            :class="[
              'flex flex-col lg:flex-row items-center gap-2 lg:gap-4 absolute lg:relative left-0 right-0 lg:left-auto lg:right-auto bg-white top-[73px] lg:top-auto bottom-0 lg:bottom-auto z-10 transition-all duration-200 px-4 lg:translate-x-0',
              isOpen ? 'translate-x-0' : '-translate-x-full',
            ]"
          >
            <div
              v-for="(menu, i) in menuItems"
              :key="i"
              class="relative group w-full lg:w-auto"
            >
              <div
                class="flex items-center justify-between lg:justify-start cursor-pointer py-3 hover:underline w-full lg:w-auto"
              >
                <NuxtLink
                  :to="menu.to"
                  class="font-normal text-base text-gray-800"
                >
                  {{ menu.title }}
                </NuxtLink>
                <ChevronDown v-if="menu.items" class="ml-1" />
              </div>

              <!-- Submenu -->
              <div
                v-if="menu.items"
                class="absolute left-0 w-80 bg-white shadow-lg rounded-md opacity-0 invisible group-hover:visible group-hover:opacity-100 transition-all duration-200 z-10"
              >
                <NuxtLink
                  v-for="(subItem, idx) in menu.items"
                  :key="idx"
                  :to="subItem.to"
                  class="block px-4 py-2.5 text-gray-700 hover:bg-[#1ea1db] hover:text-white"
                >
                  {{ subItem.title }}
                </NuxtLink>
              </div>
            </div>
            <button
              class="eligibility-btn relative isolate py-3 px-6 rounded-xl border-0 bg-white font-semibold text-base cursor-pointer text-transparent bg-gradient-to-b from-[#13447e] to-[#00bdff] bg-clip-text before:absolute before:inset-0 before:rounded-[12px] before:p-[1px] before:bg-gradient-to-b before:from-[#1ea1db] before:to-[#0c0092] before:z-[-1] lg:hidden w-full"
            >
              Check Your Eligibility
            </button>
          </div>

          <div class="flex items-center gap-4">
            <button
              class="eligibility-btn relative isolate py-3 px-6 rounded-xl border-0 bg-white font-semibold text-base cursor-pointer text-transparent bg-gradient-to-b from-[#13447e] to-[#00bdff] bg-clip-text before:absolute before:inset-0 before:rounded-[12px] before:p-[1px] before:bg-gradient-to-b before:from-[#1ea1db] before:to-[#0c0092] before:z-[-1] hidden lg:block"
            >
              Check Your Eligibility
            </button>
            <button>
              <img src="/icons/solar_cart-check-bold.svg" alt="Cart" />
            </button>
            <button class="lg:hidden" @click="isOpen = !isOpen">
              <X v-if="isOpen" />
              <TextAlignJustify v-else />
            </button>
          </div>
        </div>
      </nav>
    </div>
  </section>
</template>

<script setup>
import { ChevronDown, TextAlignJustify, X } from "lucide-vue-next";

const menuItems = ref([
  {
    title: "What we do",
    to: "/",
    items: [
      {
        title: "Study & Career Consultancy",
        to: "/",
      },
      {
        title: "Education Marketing Management",
        to: "/",
      },
      {
        title: "Partnership Support (B2B)",
        to: "/",
      },
      {
        title: "Global Study Tour",
        to: "/",
      },
      {
        title: "Government & Corporate Training",
        to: "/",
      },
      {
        title: "EdTech Solutions",
        to: "/",
      },
    ],
  },
  {
    title: "Destination",
    to: "/",
    items: [
      {
        title: "Study in Australia",
        to: "/",
      },
      {
        title: "Study in Canada",
        to: "/",
      },
      {
        title: "Study in Denmark",
        to: "/",
      },
      {
        title: "Study in Germany",
        to: "/",
      },
      {
        title: "Study in Hungary",
        to: "/",
      },
      {
        title: "Study in Malaysia",
        to: "/",
      },
      {
        title: "Study in Netherlands",
        to: "/",
      },
      {
        title: "Study in United Kingdom",
        to: "/",
      },
    ],
  },
  {
    title: "Program",
    to: "/",
  },
  {
    title: "Scholarship",
    to: "/",
  },
  {
    title: "Language hub",
    to: "/",
    items: [
      {
        title: "German Language hub",
        to: "/",
      },
    ],
  },
  {
    title: "About Us",
    to: "/",
  },
  {
    title: "Contacts Us",
    to: "/",
  },
]);

const isOpen = ref(false);
</script>

<style scoped>
.eligibility-btn::before {
  mask: linear-gradient(#fff 0 0) content-box, linear-gradient(#fff 0 0);
  mask-composite: exclude;
}
</style>
