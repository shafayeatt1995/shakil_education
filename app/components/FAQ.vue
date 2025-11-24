<template>
  <div class="container mx-auto py-8 lg:py-16 px-2 lg:px-0">
    <div class="max-w-3xl mx-auto" data-aos="fade-up">
      <h2
        class="font-['Cabin_Sketch'] font-bold text-4xl uppercase bg-gradient-to-l from-[rgba(0,189,255,1)] to-[rgba(19,68,126,1)] bg-clip-text text-transparent text-center"
      >
        Frequently Asked Questions
      </h2>
      <p class="text-sm lg:text-base text-center text-gray-600 mt-2">
        Have questions about studying abroad? Our FAQ section gives you clear
        and simple answers to guide your journey.
      </p>
    </div>
    <div class="mt-8 max-w-4xl mx-auto" data-aos="fade-up">
      <div
        v-for="(faq, i) in faqs"
        :key="i"
        class="mb-4 bg-[#F7F7F7] rounded-xl"
      >
        <div
          class="flex justify-between gap-2 cursor-pointer p-4"
          @click="toggleFaq(i)"
        >
          <span class="font-semibold">{{ faq.question }}</span>
          <span class="text-gray-600">
            <Plus
              :class="[
                ' transition-all duration-200',
                activeFaq === i ? 'rotate-45' : '',
              ]"
            />
          </span>
        </div>
        <SlideUpDown :active="activeFaq === i" :duration="200">
          <p class="pt-3 p-4">{{ faq.answer }}</p>
        </SlideUpDown>
      </div>
    </div>
  </div>
</template>

<script setup>
import { Plus } from "lucide-vue-next";
import { ref } from "vue";
import SlideUpDown from "vue-slide-up-down";

const activeFaq = ref(0);

const toggleFaq = (i) => {
  activeFaq.value = activeFaq.value === i ? null : i;
};

const faqs = [
  {
    question: "What are the basic requirements to study abroad?",
    answer:
      "We offer study tours to various international destinations including the UK, USA, Canada, Australia, and more. Contact us for the latest destinations.",
  },
  {
    question: "When should I start preparing for my study abroad journey?",
    answer:
      "We offer study tours to various international destinations including the UK, USA, Canada, Australia, and more. Contact us for the latest destinations.",
  },
  {
    question: "How do I choose the right country and university?",
    answer:
      "We offer study tours to various international destinations including the UK, USA, Canada, Australia, and more. Contact us for the latest destinations.",
  },
  {
    question: "How much does it cost to study abroad?",
    answer:
      "We offer study tours to various international destinations including the UK, USA, Canada, Australia, and more. Contact us for the latest destinations.",
  },
  {
    question: "Are there scholarships available for international students?",
    answer:
      "We offer study tours to various international destinations including the UK, USA, Canada, Australia, and more. Contact us for the latest destinations.",
  },
  {
    question: "Can I work while studying abroad?",
    answer:
      "We offer study tours to various international destinations including the UK, USA, Canada, Australia, and more. Contact us for the latest destinations.",
  },
  {
    question: "What is the process of applying for a student visa?",
    answer:
      "We offer study tours to various international destinations including the UK, USA, Canada, Australia, and more. Contact us for the latest destinations.",
  },
  {
    question: "How long does it take to get admission confirmation?",
    answer:
      "We offer study tours to various international destinations including the UK, USA, Canada, Australia, and more. Contact us for the latest destinations.",
  },
  {
    question: "Will studying abroad improve my career opportunities?",
    answer:
      "We offer study tours to various international destinations including the UK, USA, Canada, Australia, and more. Contact us for the latest destinations.",
  },
  {
    question:
      "What kind of support can I expect during the application process?",
    answer:
      "We offer study tours to various international destinations including the UK, USA, Canada, Australia, and more. Contact us for the latest destinations.",
  },
];
</script>
