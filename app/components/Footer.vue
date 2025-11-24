<template>
  <footer class="bg-[#13447E] bg-[url('/images/footer-bg.png')]">
    <div class="container mx-auto py-8 text-white px-4 lg:px-0">
      <div class="flex flex-col items-center">
        <img src="/images/footer-logo.png" alt="" class="w-32" />
        <p class="text-white">Your Bright Future is Just one Flight Away</p>
        <div class="flex justify-center gap-4 mt-3">
          <a href="#">
            <img src="/icons/linkedin.svg" alt="" class="size-6" />
          </a>
          <a href="#">
            <img src="/icons/x.svg" alt="" class="size-6" />
          </a>
          <a href="#">
            <img src="/icons/facebook.svg" alt="" class="size-6" />
          </a>
          <a href="#">
            <img src="/icons/instagram.svg" alt="" class="size-6" />
          </a>
          <a href="#">
            <img src="/icons/youtube.svg" alt="" class="size-6" />
          </a>
        </div>
      </div>
      <div
        class="grid grid-cols-1 lg:grid-cols-7 gap-8 lg:gap-5 text-white mt-16"
      >
        <div>
          <h3
            class="uppercase font-semibold border-b border-[#1EA1DB] inline-block"
          >
            Quick Veiw
          </h3>
          <ul class="mt-3">
            <li
              v-for="link in quickLinks"
              :key="link.text"
              class="hover:translate-x-1.5 transition-all duration-200"
            >
              <a :href="link.href" class="text-sm">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div>
          <h3
            class="uppercase font-semibold border-b border-[#1EA1DB] inline-block"
          >
            Quick Veiw
          </h3>
          <ul class="mt-3">
            <li
              v-for="link in quickLinks"
              :key="link.text"
              class="hover:translate-x-1.5 transition-all duration-200"
            >
              <a :href="link.href" class="text-sm">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div>
          <h3
            class="uppercase font-semibold border-b border-[#1EA1DB] inline-block"
          >
            Quick Veiw
          </h3>
          <ul class="mt-3">
            <li
              v-for="link in quickLinks"
              :key="link.text"
              class="hover:translate-x-1.5 transition-all duration-200"
            >
              <a :href="link.href" class="text-sm">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div>
          <h3
            class="uppercase font-semibold border-b border-[#1EA1DB] inline-block"
          >
            Important Links
          </h3>
          <ul class="mt-3">
            <li
              v-for="link in importantLinks"
              :key="link.text"
              class="hover:translate-x-1.5 transition-all duration-200"
            >
              <a :href="link.href" class="text-sm">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div>
          <h3
            class="uppercase font-semibold border-b border-[#1EA1DB] inline-block"
          >
            Our Services
          </h3>
          <ul class="mt-3">
            <li
              v-for="link in services"
              :key="link.text"
              class="hover:translate-x-1.5 transition-all duration-200"
            >
              <a :href="link.href" class="text-sm">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div>
          <h3
            class="uppercase font-semibold border-b border-[#1EA1DB] inline-block"
          >
            Study destinations
          </h3>
          <ul class="mt-3">
            <li
              v-for="link in studyDestinations"
              :key="link.text"
              class="hover:translate-x-1.5 transition-all duration-200"
            >
              <a :href="link.href" class="text-sm">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div>
          <h3
            class="uppercase font-semibold border-b border-[#1EA1DB] inline-block"
          >
            Contact Us
          </h3>
          <ul class="mt-3">
            <li
              v-for="link in contactUs"
              :key="link.text"
              class="hover:translate-x-1.5 transition-all duration-200"
            >
              <a :href="'tel:' + link.href" class="text-sm">{{ link.text }}</a>
            </li>
          </ul>
        </div>
      </div>

      <hr class="mt-10 mb-5" />
      <div>
        <p class="text-center font-semibold">Our Office</p>
        <div class="grid grid-cols-1 lg:grid-cols-4 gap-5 mt-5">
          <div v-for="office in office" :key="office.name" class="mt-1">
            <p
              class="uppercase font-semibold border-b border-[#1EA1DB] inline-block text-sm"
            >
              {{ office.name }}
            </p>
            <p class="text-xs mt-2">{{ office.address }}</p>
          </div>
        </div>
      </div>
      <p class="text-center mt-10 text-xs">
        Copyright@2025 Shakil Education Group All right reserved
      </p>
    </div>
  </footer>
</template>

<script setup>
const quickLinks = [
  { text: "News", href: "#" },
  { text: "Event", href: "#" },
  { text: "Career", href: "#" },
  { text: "Contact Us", href: "#" },
  { text: "About Us", href: "#" },
];

const importantLinks = [
  { text: "Study Abroad", href: "#" },
  { text: "Programs", href: "#" },
  { text: "Scholarships", href: "#" },
  { text: "IELTS", href: "#" },
  { text: "German Language", href: "#" },
];

const services = [
  { text: "Study & Career Consultancy", href: "#" },
  { text: "Education Marketing Management", href: "#" },
  { text: "Partnership Support(B2B)", href: "#" },
  { text: "Global Study Tour", href: "#" },
  { text: "Government & Corporate Training", href: "#" },
  { text: "EdTech Solution", href: "#" },
];

const studyDestinations = [
  { text: "Study in Australia", href: "#" },
  { text: "Study in Canada", href: "#" },
  { text: "Study in Denmark", href: "#" },
  { text: "Study in Germany", href: "#" },
  { text: "Study in Malaysia", href: "#" },
  { text: "Study in The UK", href: "#" },
];

const contactUs = [
  { text: "+880 1880 000091", href: "+8801880000091" },
  { text: "+880 1880 000092", href: "+8801880000092" },
  { text: "+880 1880 000093", href: "+8801880000093" },
  { text: "+880 1880 000094", href: "+8801880000094" },
  { text: "+880 1880 000095", href: "+8801880000095" },
];

const office = [
  {
    name: "Dhaka",
    address:
      "Lift-3 & 5, House #63/C, Mir Taj Square, New Lazz Pharma Building, (Dhanmondi-32 Signal, West Panthapath Road), Dhaka-1205, Bangladesh",
  },
  {
    name: "Sylhet",
    address:
      "811, Level 8 , Al Hamra Shopping City, Zindabazar, Sylhet, Bangladesh",
  },
  {
    name: "Germany",
    address: "SHAKIL GmbH, Marktstraße 27, 41236 Mönchengladbach, Germany",
  },
  {
    name: "UK",
    address: "SHAKIL GmbH, Marktstraße 27, 41236 Mönchengladbach, Germany",
  },
];
</script>

<script setup></script>
