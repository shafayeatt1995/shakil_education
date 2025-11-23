<template>
  <div class="min-h-screen bg-white">
    <!-- Hero Section -->
    <Hero />

    <!-- Section 2: Statistics and Features -->
    <section
      class="w-full max-w-[1440px] mx-auto bg-white"
      style="height: 1281px"
    >
      <!-- Statistics -->
      <div
        class="pt-[691px] px-[127px] flex justify-between items-center gap-5"
      >
        <div
          class="w-[237px] flex items-center gap-5 border-r border-[#E5E7EB] pr-5"
        >
          <div class="flex flex-col">
            <span
              class="text-[64px] font-bold font-['Cabin_Sketch'] leading-[1.171] text-transparent bg-clip-text bg-gradient-to-r from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)]"
              >12k+</span
            >
            <span
              class="text-xl font-normal font-['Cabin_Sketch'] leading-[1.171] text-black w-[99px]"
              >Happy travelers</span
            >
          </div>
        </div>
        <div
          class="w-[237px] flex items-center gap-5 border-r border-[#E5E7EB] pr-5"
        >
          <div class="flex flex-col">
            <span
              class="text-[64px] font-bold font-['Cabin_Sketch'] leading-[1.171] text-transparent bg-clip-text bg-gradient-to-r from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)]"
              >10k+</span
            >
            <span
              class="text-xl font-normal font-['Cabin_Sketch'] leading-[1.171] text-black w-[88px]"
              >Flights booked</span
            >
          </div>
        </div>
        <div
          class="w-[237px] flex items-center gap-5 border-r border-[#E5E7EB] pr-5"
        >
          <div class="flex flex-col">
            <span
              class="text-[64px] font-bold font-['Cabin_Sketch'] leading-[1.171] text-transparent bg-clip-text bg-gradient-to-r from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)]"
              >5k+</span
            >
            <span
              class="text-xl font-normal font-['Cabin_Sketch'] leading-[1.171] text-black w-[110px]"
              >Tours organized</span
            >
          </div>
        </div>
        <div class="w-[237px] flex items-center gap-5">
          <div class="flex flex-col">
            <span
              class="text-[64px] font-bold font-['Cabin_Sketch'] leading-[1.171] text-transparent bg-clip-text bg-gradient-to-r from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)]"
              >8k+</span
            >
            <span
              class="text-xl font-normal font-['Cabin_Sketch'] leading-[1.171] text-black"
              >Hotel stays</span
            >
          </div>
        </div>
      </div>

      <!-- Travel Companion Section -->
      <div class="relative mt-[539px] ml-[57px] w-[1307px] h-[667px]">
        <!-- Yellow Circle -->
        <div
          class="absolute left-[1238px] top-[257px] w-[65px] h-[65px] rounded-full bg-[#FFEA2F]"
        ></div>

        <!-- Vector Decoration -->
        <div class="absolute left-[26px] top-[104px] w-[441.41px] h-[494.71px]">
          <img
            src="/images/vector-decoration.svg"
            alt="Vector"
            class="w-full h-full"
          />
        </div>

        <!-- Travel Companion Card -->
        <div
          class="absolute left-[24px] top-[460px] w-[1279px] h-[207px] bg-[#13447E] rounded-[24px] flex items-center justify-between px-[365px]"
        >
          <p class="text-[32px] font-bold leading-[1.5] uppercase text-white">
            Your travel companion that carries<br />all the information
          </p>
          <div class="w-[332px] h-[498px] -mt-[291px]">
            <img
              src="/images/travel-girl.png"
              alt="Travel girl"
              class="w-full h-full object-cover"
            />
          </div>
        </div>

        <!-- Airplane -->
        <div class="absolute left-[173px] top-[469px] w-[194.48px] h-[94.12px]">
          <img
            src="/images/airplane-3a90f1.png"
            alt="Airplane"
            class="w-full h-full object-contain"
          />
        </div>

        <!-- Image 109 -->
        <div class="absolute left-[14px] top-[276px] w-[282px] h-[298px]">
          <img
            src="/images/image-109-108923.png"
            alt="Image"
            class="w-full h-full object-cover"
          />
        </div>

        <!-- Cloud -->
        <div class="absolute left-[49px] top-[514px] w-[211px] h-[112px]">
          <img
            src="/images/cloud-5214e9.png"
            alt="Cloud"
            class="w-full h-full object-cover"
          />
        </div>

        <!-- Small Cloud -->
        <div class="absolute left-[1024px] top-[298px] w-[70px] h-[70px]">
          <img
            src="/images/cloud-small.svg"
            alt="Cloud"
            class="w-full h-full"
          />
        </div>
      </div>

      <!-- Features Section -->
      <div class="mt-[61px] ml-[84px] flex gap-[34px]">
        <div class="w-[622px] flex flex-col gap-8">
          <div class="flex flex-col gap-4">
            <h2
              class="text-[48px] font-bold font-['Cabin_Sketch'] leading-[1.171] uppercase text-transparent bg-clip-text bg-gradient-to-r from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)]"
            >
              Discover the world, one journey at a time.
            </h2>
            <p class="text-base font-normal leading-[1.5] text-[#000000]">
              From breathtaking landscapes to cultural wonders, we craft
              journeys that bring your dream destinations to life. Whether
              you're planning a relaxing getaway or an adventure-filled
              expedition, our team ensures every detail is taken care of.
            </p>
          </div>

          <div class="flex flex-col gap-2">
            <div class="flex items-center gap-1">
              <svg
                class="w-5 h-5 flex-shrink-0"
                viewBox="0 0 20 20"
                fill="none"
              >
                <circle cx="10" cy="10" r="9" fill="#FFABCC" />
                <path
                  d="M6 10L9 13L14 7"
                  stroke="#13447E"
                  stroke-width="1.2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
              <span class="text-base font-normal text-[#6B7280]"
                >Premium Stays & Exclusive Deals</span
              >
            </div>
            <div class="flex items-center gap-1">
              <svg
                class="w-5 h-5 flex-shrink-0"
                viewBox="0 0 20 20"
                fill="none"
              >
                <circle cx="10" cy="10" r="9" fill="#FFABCC" />
                <path
                  d="M6 10L9 13L14 7"
                  stroke="#13447E"
                  stroke-width="1.2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
              <span class="text-base font-normal text-[#6B7280]"
                >Tailored Packages for Every Traveler</span
              >
            </div>
            <div class="flex items-center gap-1">
              <svg
                class="w-5 h-5 flex-shrink-0"
                viewBox="0 0 20 20"
                fill="none"
              >
                <circle cx="10" cy="10" r="9" fill="#FFABCC" />
                <path
                  d="M6 10L9 13L14 7"
                  stroke="#13447E"
                  stroke-width="1.2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
              <span class="text-base font-normal text-[#6B7280]"
                >Unmatched Support Before & During Trips</span
              >
            </div>
          </div>
        </div>

        <!-- Feature Image -->
        <div class="w-[624px] h-[478px]">
          <img
            src="/images/tour-package-images.png"
            alt="Features"
            class="w-full h-full object-cover rounded-lg"
          />
        </div>
      </div>
    </section>

    <!-- Section 5: Academic Excellence -->
    <section
      class="w-full max-w-[1440px] mx-auto bg-white"
      style="height: 781px"
    >
      <div class="relative">
        <!-- Background Images -->
        <div
          class="absolute left-[-36px] top-[325px] w-[1500px] flex items-center gap-2"
        >
          <div
            class="flex-1 h-full py-5 px-6 flex flex-col justify-center gap-8"
          >
            <img
              src="/images/university-1.png"
              alt="University 1"
              class="w-full h-full object-cover rounded-lg"
            />
          </div>
          <div class="h-full py-5 px-6 flex flex-col justify-center gap-8">
            <img
              src="/images/university-2.png"
              alt="University 2"
              class="w-full h-full object-cover rounded-lg"
            />
          </div>
          <div class="h-full py-5 px-6 flex flex-col justify-center gap-8">
            <img
              src="/images/university-3.png"
              alt="University 3"
              class="w-full h-full object-cover rounded-lg"
            />
          </div>
          <div class="h-full py-5 px-6 flex flex-col justify-center gap-8">
            <img
              src="/images/university-4.png"
              alt="University 4"
              class="w-full h-full object-cover rounded-lg"
            />
          </div>
        </div>

        <!-- Gradient Overlay -->
        <div
          class="absolute left-[-6px] top-[314px] w-[1440px] h-[455px] bg-gradient-to-b from-white via-transparent to-white blur-[40px]"
        ></div>

        <!-- Title -->
        <div class="absolute left-[228px] top-[126px] w-[984px] h-[150px]">
          <h2
            class="text-[64px] font-bold font-['Cabin_Sketch'] leading-[1.171] uppercase text-center text-transparent bg-clip-text bg-gradient-to-r from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)]"
          >
            Academic Excellence Meets Cultural Discovery
          </h2>
        </div>

        <!-- Card -->
        <div
          class="absolute left-[375px] top-[416px] w-[690px] h-[180px] bg-[rgba(255,255,255,0.8)] rounded-xl p-5 flex flex-col justify-center gap-[23px]"
        >
          <h3
            class="text-[32px] font-bold leading-[1.5] uppercase text-center text-black"
          >
            Elite University Visits
          </h3>
          <p
            class="text-base font-normal leading-[1.5] uppercase text-center text-black"
          >
            Tour Harvard, MIT, Stanford, Oxford, and other world-leading
            institutions with exclusive campus access, library tours, and
            student interactions
          </p>
        </div>

        <!-- Navigation Arrows -->
        <div
          class="absolute left-[354px] top-[484px] w-[42px] h-[41px] bg-[#E5E7EB] rounded-full flex items-center justify-center"
        >
          <svg class="w-[18px] h-[36px]" fill="none" viewBox="0 0 18 36">
            <path
              d="M2.33 8.45L11.05 19.09L13.38 27.55"
              stroke="#13447E"
              stroke-width="2"
            />
          </svg>
        </div>
        <div
          class="absolute left-[1044px] top-[484px] w-[42px] h-[41px] bg-[#E5E7EB] rounded-full flex items-center justify-center"
        >
          <svg class="w-[18px] h-[36px]" fill="none" viewBox="0 0 18 36">
            <path
              d="M4.63 8.46L15.68 19.09L13.38 27.55"
              stroke="#13447E"
              stroke-width="2"
            />
          </svg>
        </div>
      </div>
    </section>

    <!-- Section 4: Tour Packages -->
    <section
      class="w-full max-w-[1440px] mx-auto bg-white"
      style="height: 1145px"
    >
      <div class="pt-[56px] px-[361px] flex flex-col items-center gap-2">
        <div class="flex items-center justify-center gap-[10px] mb-2">
          <span
            class="text-base font-normal font-['Cabin_Sketch'] text-[#13447E]"
            >Discover the places travelers love the most!</span
          >
        </div>
        <div class="w-[718px] flex flex-col items-center gap-3">
          <h2
            class="text-[64px] font-bold font-['Cabin_Sketch'] leading-[1.171] uppercase text-transparent bg-clip-text bg-gradient-to-r from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)]"
          >
            Tour Packages Section
          </h2>
          <p class="text-base font-normal text-[#6B7280] text-center">
            From breathtaking landscapes to vibrant cultures, these destinations
            are handpicked to give you unforgettable memories.
          </p>
        </div>
      </div>

      <!-- Package Tabs -->
      <div class="mt-[273px] ml-[153px] w-[1134px] h-[800px]">
        <div class="flex justify-between items-center gap-2 mb-[94px]">
          <button
            class="px-[60px] py-8 rounded-t-[40px] bg-[#F2F2F7] text-[#13447E] text-xl font-bold"
          >
            USA Package 1
          </button>
          <button
            class="px-10 py-5 rounded-t-[32px] bg-[#E1EDFA] text-[#13447E] text-base font-semibold"
          >
            USA Package 2
          </button>
          <button
            class="px-10 py-5 rounded-t-[32px] bg-[#E1EDFA] text-[#13447E] text-base font-semibold"
          >
            EU Package 1
          </button>
          <button
            class="px-10 py-5 rounded-t-[32px] bg-[#E1EDFA] text-[#13447E] text-base font-semibold"
          >
            EU Package 2
          </button>
        </div>

        <!-- Package Card -->
        <div
          class="w-[878px] h-[706px] bg-[#F2F2F7] rounded-[32px] p-5 flex gap-10"
        >
          <div class="w-[624px] flex flex-col gap-3">
            <img
              src="/images/tour-package-main-462081.png"
              alt="Tour"
              class="w-full h-[281px] object-cover rounded-lg"
            />
            <div class="flex gap-2">
              <img
                src="/images/tour-package-images.png"
                alt="Tour 1"
                class="flex-1 h-full object-cover rounded-lg"
              />
              <img
                src="/images/tour-package-images-2.png"
                alt="Tour 2"
                class="flex-1 h-full object-cover rounded-lg"
              />
            </div>
          </div>

          <div class="flex-1 flex flex-col gap-3">
            <div class="pb-4 border-b border-[#E5E7EB]">
              <span class="text-base font-bold text-[#13447E]">Day 1</span>
            </div>
            <div class="flex flex-col gap-6">
              <div class="flex flex-col gap-2">
                <h3
                  class="text-[32px] font-bold leading-[1.5] uppercase text-[#13447E]"
                >
                  Arrival & City Tour
                </h3>
                <p class="text-base font-normal text-[#000000]">
                  Begin your journey with a comprehensive city tour, exploring
                  iconic landmarks and getting acquainted with the vibrant
                  culture.
                </p>
              </div>
              <div
                class="text-base font-normal text-[#6B7280] whitespace-pre-line"
              >
                Airport pickup and hotel check-in Welcome dinner at a local
                restaurant Evening city lights tour Meet and greet with tour
                guide
              </div>
            </div>
          </div>
        </div>

        <!-- Book Button -->
        <button
          class="absolute left-[716px] top-[499px] w-[394px] h-[52px] bg-gradient-to-r from-[rgba(19,68,126,1)] to-[rgba(0,189,255,1)] rounded-lg text-white text-xl font-normal font-['Cabin_Sketch']"
        >
          Book This Tour today
        </button>

        <!-- Day Navigation -->
        <div
          class="absolute left-[40px] top-[589px] flex items-center gap-[7px]"
        >
          <button
            class="px-5 py-5 rounded-[78px] bg-[#13447E] text-white text-base font-semibold shadow-[0px_-5px_3px_0px_rgba(151,215,255,0.2)]"
          >
            Day 1
          </button>
          <button
            class="px-5 py-5 rounded-[78px] bg-white text-[#000000] text-base font-semibold shadow-[0px_-5px_3px_0px_rgba(151,215,255,0.2)]"
          >
            Day 2
          </button>
          <button
            class="px-5 py-5 rounded-[78px] bg-white text-[#000000] text-base font-semibold shadow-[0px_-5px_3px_0px_rgba(151,215,255,0.2)]"
          >
            Day 3
          </button>
          <button
            class="px-5 py-5 rounded-[78px] bg-white text-[#000000] text-base font-semibold shadow-[0px_-5px_3px_0px_rgba(151,215,255,0.2)]"
          >
            Day 4
          </button>
          <button
            class="px-5 py-5 rounded-[78px] bg-white text-[#000000] text-base font-semibold shadow-[0px_-5px_3px_0px_rgba(151,215,255,0.2)]"
          >
            Day 5
          </button>
          <button
            class="px-5 py-5 rounded-[78px] bg-white text-[#000000] text-base font-semibold shadow-[0px_-5px_3px_0px_rgba(151,215,255,0.2)]"
          >
            Day 6
          </button>
          <button
            class="px-5 py-5 rounded-[78px] bg-white text-[#000000] text-base font-semibold shadow-[0px_-5px_3px_0px_rgba(151,215,255,0.2)]"
          >
            Day 7
          </button>
          <button
            class="px-5 py-5 rounded-[78px] bg-white text-[#000000] text-base font-semibold shadow-[0px_-5px_3px_0px_rgba(151,215,255,0.2)]"
          >
            Day 8
          </button>
          <button
            class="px-5 py-5 rounded-[78px] bg-white text-[#000000] text-base font-semibold shadow-[0px_-5px_3px_0px_rgba(151,215,255,0.2)]"
          >
            Day 9
          </button>
          <button
            class="px-5 py-5 rounded-[78px] bg-white text-[#000000] text-base font-semibold shadow-[0px_-5px_3px_0px_rgba(151,215,255,0.2)]"
          >
            Day 10
          </button>
          <button
            class="px-5 py-5 rounded-[78px] bg-white text-[#000000] text-base font-semibold shadow-[0px_-5px_3px_0px_rgba(151,215,255,0.2)]"
          >
            Day 11
          </button>
        </div>
      </div>
    </section>

    <!-- Popular Destinations Section -->
    <section
      class="w-full max-w-[1440px] mx-auto bg-white"
      style="height: 921px"
    >
      <div class="relative">
        <!-- Icons -->
        <div class="absolute left-[507px] top-[18px] w-[60px] h-[60px]">
          <img src="/images/plane-icon.svg" alt="Plane" class="w-full h-full" />
        </div>
        <div class="absolute left-[813px] top-[600px] w-[86.49px] h-[86.49px]">
          <img
            src="/images/camera-icon.svg"
            alt="Camera"
            class="w-full h-full"
          />
        </div>
        <div class="absolute left-[148px] top-[554px] w-[78.17px] h-[78.17px]">
          <img
            src="/images/luggage-icon.svg"
            alt="Luggage"
            class="w-full h-full"
          />
        </div>

        <!-- Content -->
        <div
          class="absolute left-[80px] top-[94px] w-[624px] flex flex-col gap-5"
        >
          <h2
            class="text-[64px] font-bold font-['Cabin_Sketch'] leading-[1.171] uppercase text-transparent bg-clip-text bg-gradient-to-r from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)]"
          >
            Why Travel with Shakil Education Group?
          </h2>
          <div class="flex flex-col gap-5">
            <p class="text-base font-normal text-[#6B7280]">
              we believe travel is more than just visiting new places—it's about
              creating unforgettable experiences.
            </p>
            <button
              class="w-[261px] h-[52px] bg-gradient-to-r from-[rgba(19,68,126,1)] to-[rgba(0,189,255,1)] rounded-lg text-white text-xl font-normal font-['Cabin_Sketch']"
            >
              See Our Packages
            </button>
          </div>
        </div>

        <!-- Background Image -->
        <div
          class="absolute left-[736px] top-[78px] w-[624px] h-[474px] rounded-2xl overflow-hidden"
        ></div>

        <!-- Features -->
        <div class="absolute left-[79px] top-[698px] flex gap-[33px]">
          <div class="w-[405px] flex flex-col gap-5">
            <h3 class="text-2xl font-bold text-[#13447E]">Trust</h3>
            <p class="text-base font-normal text-[#000000]">
              Certified Tour Operator, Official Academic Partner, Reliable
              Travel Companion
            </p>
          </div>
          <div class="w-[405px] flex flex-col gap-5">
            <h3 class="text-2xl font-bold text-[#13447E]">Expertise</h3>
            <p class="text-base font-normal text-[#000000]">
              Expert Guides, Experienced Coordinators, Educational Itinerary,
              University Visits
            </p>
          </div>
          <div class="w-[405px] flex flex-col gap-5">
            <h3 class="text-2xl font-bold text-[#13447E]">Value</h3>
            <p class="text-base font-normal text-[#000000]">
              All-inclusive Packages, Transparent Pricing, Group Discounts
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Section 3: Gallery -->
    <section
      class="w-full max-w-[1440px] mx-auto bg-white"
      style="height: 1179px"
    >
      <div class="relative">
        <!-- Vector Decoration -->
        <div
          class="absolute left-[1100.07px] top-[696px] w-[308.42px] h-[358.65px]"
        >
          <img
            src="/images/vector-gallery.svg"
            alt="Vector"
            class="w-full h-full"
          />
        </div>

        <!-- Title -->
        <div
          class="absolute left-[1060px] top-[925px] w-[303px] flex flex-col items-center gap-1"
        >
          <h2 class="text-[64px] font-bold uppercase text-[#13447E]">
            Gallery
          </h2>
          <p class="text-base font-normal text-[#6B7280] text-center">
            See exciting photos from our photo gallery<br />& choose your next
            trip easily
          </p>
        </div>

        <!-- Gallery Images -->
        <div
          class="absolute left-[80px] top-[106px] w-[296px] h-[467px] rounded-[20px] overflow-hidden shadow-[5px_1px_11.3px_3px_rgba(0,189,255,0.2)]"
        >
          <img
            src="/images/gallery-1-1d244e.png"
            alt="Gallery 1"
            class="w-full h-full object-cover"
          />
        </div>
        <div
          class="absolute left-[408px] top-[106px] w-[296px] h-[543px] rounded-[20px] overflow-hidden shadow-[5px_1px_11.3px_3px_rgba(0,189,255,0.2)]"
        >
          <img
            src="/images/gallery-2-295def.png"
            alt="Gallery 2"
            class="w-full h-full object-cover"
          />
        </div>
        <div
          class="absolute left-[736px] top-[509px] w-[296px] h-[543px] rounded-[20px] overflow-hidden shadow-[5px_1px_11.3px_3px_rgba(0,189,255,0.2)]"
        >
          <img
            src="/images/gallery-3.png"
            alt="Gallery 3"
            class="w-full h-full object-cover"
          />
        </div>
        <div
          class="absolute left-[1064px] top-[106px] w-[296px] h-[784px] rounded-[20px] overflow-hidden shadow-[5px_1px_11.3px_3px_rgba(0,189,255,0.2)]"
        >
          <img
            src="/images/gallery-4.png"
            alt="Gallery 4"
            class="w-full h-full object-cover"
          />
        </div>
        <div
          class="absolute left-[80px] top-[585px] w-[296px] h-[467px] rounded-[20px] overflow-hidden shadow-[5px_1px_11.3px_3px_rgba(0,189,255,0.2)]"
        >
          <img
            src="/images/university-1.png"
            alt="Gallery 5"
            class="w-full h-full object-cover"
          />
        </div>
        <div
          class="absolute left-[408px] top-[658px] w-[296px] h-[394px] rounded-[20px] overflow-hidden shadow-[5px_1px_10px_3px_rgba(0,189,255,0.2)]"
        >
          <img
            src="/images/gallery-6.png"
            alt="Gallery 6"
            class="w-full h-full object-cover"
          />
        </div>
        <div
          class="absolute left-[736px] top-[106px] w-[296px] h-[394px] rounded-[20px] overflow-hidden shadow-[5px_1px_11.3px_3px_rgba(0,189,255,0.2)]"
        >
          <img
            src="/images/gallery-3.png"
            alt="Gallery 7"
            class="w-full h-full object-cover"
          />
        </div>
      </div>
    </section>

    <!-- Testimonials Section -->
    <section
      class="w-full max-w-[1440px] mx-auto bg-white"
      style="height: 726px"
    >
      <div class="relative">
        <!-- Testimonial Cards -->
        <div
          class="absolute left-[1797px] top-[192px] w-[340px] bg-[#F7F7F7] rounded-[30px] p-8 flex flex-col gap-10"
        >
          <div class="flex items-center gap-[91px]">
            <div class="flex items-center gap-[10px]">
              <div class="w-[70px] h-[70px] rounded-full overflow-hidden">
                <img
                  src="/images/testimonial-avatar-1.png"
                  alt="Avatar"
                  class="w-full h-full object-cover"
                />
              </div>
              <div class="flex flex-col gap-2">
                <span
                  class="text-2xl font-semibold font-['Public_Sans'] text-[#000000]"
                  >Guy Hawkins</span
                >
                <span class="text-base font-normal text-[#2C2C2C]"
                  >21st August 2025</span
                >
              </div>
            </div>
            <img
              src="/images/google-icon.svg"
              alt="Google"
              class="w-[33px] h-[33px]"
            />
          </div>
          <div class="flex flex-col gap-[19px]">
            <div class="flex items-center gap-[5px]">
              <img
                src="/images/stars.svg"
                alt="Stars"
                class="w-[135px] h-[19px]"
              />
            </div>
            <p class="text-base font-medium text-[#888585]">
              Thanks to SEG, my dream of studying abroad came true. Their
              guidance made the whole process smooth and stress-free. I'm now
              studying at University of Manilla, Australia, and couldn't be
              happier!
            </p>
          </div>
        </div>

        <!-- More testimonial cards would go here, but I'll add a few key ones -->
        <div class="absolute left-[80px] top-[92px] w-[1360px] h-[441px]">
          <div class="flex items-center gap-5">
            <div class="flex-1">
              <h2
                class="text-[32px] font-semibold text-transparent bg-clip-text bg-gradient-to-r from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)] mb-6"
              >
                What Our Students Say
              </h2>
              <button
                class="px-4 py-2 rounded-[18px] bg-[#EFFAFF] border border-[#C9EFFF] text-[#00BDFF] text-sm font-medium flex items-center gap-2"
              >
                Review us on
                <img
                  src="/images/google-icon.svg"
                  alt="Google"
                  class="w-4 h-4"
                />
              </button>
            </div>
            <div class="flex gap-5">
              <!-- Navigation arrows would go here -->
            </div>
          </div>
        </div>

        <!-- Apply Now Button -->
        <button
          class="absolute left-[636px] top-[588px] h-[52px] px-10 bg-gradient-to-r from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)] rounded text-white text-base font-semibold"
        >
          Apply Now
        </button>
      </div>
    </section>

    <!-- CTA Section -->
    <section
      class="w-full max-w-[1440px] mx-auto bg-white"
      style="height: 304px"
    >
      <div class="h-full flex items-center justify-center px-[188px] py-[18px]">
        <div
          class="w-[1063px] bg-[#FAFAFA] rounded-2xl shadow-[0px_0px_4px_0px_rgba(0,0,0,0.2)] p-10 flex items-center justify-center gap-10"
        >
          <div class="flex-1 flex flex-col gap-2">
            <h2
              class="text-[32px] font-semibold uppercase text-transparent bg-clip-text bg-gradient-to-r from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)]"
            >
              Let's Make it To Your Dream Country With<br />Shakil Education
              Groupe
            </h2>
            <p class="text-sm font-normal text-[rgba(0,0,0,0.6)]">
              Get personalized guidance on admissions, scholarships, and visas —
              free of cost.
            </p>
          </div>
          <button
            class="h-[52px] px-10 bg-gradient-to-r from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)] rounded text-white text-xl font-normal font-['Cabin_Sketch']"
          >
            Book Your Tour
          </button>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="w-full bg-[#000000]">
      <div class="w-full max-w-[1440px] mx-auto px-[328px] py-8 lg:py-16">
        <!-- FAQ Section -->
        <div class="flex flex-col items-center gap-[66px] mb-10">
          <div class="flex flex-col items-center gap-[15px]">
            <h2
              class="text-[38px] font-bold font-['Cabin_Sketch'] leading-[1.5] text-transparent bg-clip-text bg-gradient-to-r from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)]"
            >
              Frequently Asked Questions
            </h2>
            <p class="text-base font-normal text-[#4D4D4D] text-center">
              Have questions about studying abroad?<br />Our FAQ section gives
              you clear and simple answers to guide your journey.
            </p>
          </div>

          <!-- FAQ Items -->
          <div class="w-[776px] flex flex-col gap-3">
            <div class="bg-[#F7F7F7] rounded-2xl p-6">
              <div class="flex justify-between items-center">
                <span class="text-base font-medium text-[#2C2C2C]"
                  >Who can join the study tour?</span
                >
                <svg class="w-7 h-7" fill="none" viewBox="0 0 28 28">
                  <path
                    d="M10.02 10.02L18.02 18.02M18.02 10.02L10.02 18.02"
                    stroke="#2C2C2C"
                    stroke-width="1.6"
                  />
                </svg>
              </div>
              <p class="mt-5 text-base font-normal text-[#4D4D4D]">
                Our study tours are open to students, teachers, and academic
                institutions who want international exposure.
              </p>
            </div>
            <!-- More FAQ items would go here -->
          </div>
        </div>

        <!-- Footer Content -->
        <div class="flex flex-col items-center gap-[69px]">
          <div class="flex flex-col items-center gap-1.5">
            <img
              src="/images/footer-logo.svg"
              alt="Logo"
              class="w-[124.5px] h-[39.78px]"
            />
            <p class="text-[10.5px] font-normal font-['Ubuntu'] text-white">
              Your Bright Future is Just one Flight Away
            </p>
          </div>

          <!-- Footer Links -->
          <div class="w-full flex justify-between items-start gap-[94px]">
            <div class="flex flex-col gap-[18px]">
              <div class="flex flex-col gap-0.5">
                <span
                  class="text-xs font-medium font-['Ubuntu'] uppercase text-white"
                  >Quick View</span
                >
                <div class="w-full h-0.5 bg-[#1EA1DB]"></div>
              </div>
              <div class="flex flex-col gap-[6.75px]">
                <a
                  href="#"
                  class="text-[10.5px] font-normal font-['Ubuntu'] text-white"
                  >News</a
                >
                <a
                  href="#"
                  class="text-[10.5px] font-normal font-['Ubuntu'] text-white"
                  >Event</a
                >
                <a
                  href="#"
                  class="text-[10.5px] font-normal font-['Ubuntu'] text-white"
                  >Career</a
                >
                <a
                  href="#"
                  class="text-[10.5px] font-normal font-['Ubuntu'] text-white"
                  >Contact Us</a
                >
                <a
                  href="#"
                  class="text-[10.5px] font-normal font-['Ubuntu'] text-white"
                  >About Us</a
                >
              </div>
            </div>
            <!-- More footer columns would go here -->
          </div>

          <!-- Copyright -->
          <p class="text-[10.5px] font-normal text-white text-center">
            Copyright@2025 Shakil Education Group All right reserved
          </p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
// Component logic can be added here
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&family=Cabin+Sketch:wght@400;700&family=Ubuntu:wght@400;500;700&family=Public+Sans:wght@600&display=swap");
</style>
