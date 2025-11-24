<template>
  <section class="container mx-auto py-8 lg:py-16">
    <div class="max-w-3xl mx-auto" data-aos="fade-up">
      <p
        class="font-['Cabin_Sketch'] text-[#13447E] text-center text-sm lg:text-base"
      >
        Discover the places travelers love the most!
      </p>
      <h2
        class="font-['Cabin_Sketch'] font-bold text-4xl lg:text-6xl uppercase text-center bg-gradient-to-r from-[#00bdff] to-[#13447e] bg-clip-text text-transparent"
      >
        Tour Packages Section
      </h2>
      <p class="text-sm lg:text-base text-center text-gray-500">
        From breathtaking landscapes to vibrant cultures, these destinations are
        handpicked to give you unforgettable memories.
      </p>
    </div>
    <div class="mt-14" data-aos="fade-up">
      <div
        class="flex gap-2 justify-between items-center max-w-4xl mx-auto whitespace-nowrap overflow-x-auto"
      >
        <button
          v-for="(pack, i) in packages"
          :key="i"
          :class="[
            ' text-[#13447E] rounded-t-3xl font-semibold transition-all duration-200 px-5',
            active === i
              ? 'bg-[#F2F2F7] text-xl w-[calc(100%+150px)] h-16 lg:h-20'
              : 'w-full h-16 bg-[#E1EDFA]',
          ]"
          @click="active = i"
        >
          {{ pack }}
        </button>
      </div>
      <div class="bg-[#F2F2F7] p-5 lg:p-10 lg:rounded-3xl max-w-7xl mx-auto">
        <div class="grid grid-cols-1 lg:grid-cols-5 gap-10 lg:gap-5">
          <div class="col-span-3 space-y-2">
            <img
              src="/images/package/1.png"
              class="rounded-xl lg:h-72 w-full"
            />
            <div class="grid grid-cols-3 gap-2 justify-between">
              <img
                src="/images/package/2.png"
                class="rounded-xl lg:h-56 w-full"
              />
              <img
                src="/images/package/3.png"
                class="rounded-xl lg:h-56 w-full"
              />
              <img
                src="/images/package/4.png"
                class="rounded-xl lg:h-56 w-full"
              />
            </div>
          </div>
          <div class="col-span-2">
            <div class="flex flex-col justify-between h-full">
              <div class="mb-10">
                <p class="font-bold text-[#13447E] mb-2">Day {{ day }}</p>
                <hr />
                <h3 class="font-bold text-[32px] text-[#13447E] mt-3">
                  Arrival & City Tour
                </h3>
                <p>
                  Begin your journey with a comprehensive city tour, exploring
                  iconic landmarks and getting acquainted with the vibrant
                  culture.
                </p>
                <ul class="list-disc text-gray-500 pl-4 mt-5">
                  <li>Airport pickup and hotel check-in</li>
                  <li>Welcome dinner at a local restaurant</li>
                  <li>Evening city lights tour</li>
                  <li>Meet and greet with tour guide</li>
                </ul>
              </div>
              <button
                class="py-4 px-8 rounded-lg bg-gradient-to-r from-[#13447e] to-[#00bdff] border-none font-['Cabin_Sketch'] font-normal text-xl text-white transition-opacity duration-200 hover:opacity-90"
              >
                Book This Tour today
              </button>
            </div>
          </div>
        </div>
        <div
          class="flex whitespace-nowrap overflow-x-auto justify-between gap-2 flex-1 mt-10 pb-5"
        >
          <button
            :class="[
              'flex w-full p-5 justify-center items-center  rounded-3xl shadow-lg transition-all duration-200',
              day === d
                ? 'bg-[#13447E] text-white'
                : 'bg-white shadow-[0px_5px_3px_rgba(151,215,255,0.2)]',
            ]"
            v-for="(d, i) in 11"
            :key="i"
            @click="day = d"
          >
            Day {{ d }}
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const day = ref(1);
const active = ref(0);
const packages = ref([
  "USA Package 1",
  "USA Package 2",
  "EU Package 1",
  "EU Package 2",
]);
</script>
