<template>
  <div class="flex flex-col items-center gap-4 overflow-hidden lg:my-[100px]">
    <h1 class="text-[36px]">Халқаро индексация базалари</h1>
    <p class="text-[20px] text-center">
      Журналимиз қуйидаги халқаро маълумот базаларида индексланган
    </p>

    <!-- Carousel -->
    <div class="relative w-full flex items-center flex-row justify-center overflow-hidden">
        <button
        @click="prev"
        class="px-4 py-2 border rounded hover:bg-gray-100 transition-colors z-10"
        >
        <i class="fa-solid fa-angle-left"></i>
    </button>
      <div
        class="flex transition-transform  duration-500 ease-in-out justify-center"
        :style="{ transform: `translateX(${translateX}px)` }"
      >
        <div
          v-for="(img, i) in images"
          :key="i"
          class="flex-shrink-0 flex justify-center items-center bg-[#E5E7EB] rounded-[10px] w-[206px] h-[128px] mx-2 transition-all duration-500"
          :class="
            i === currentIndex ? 'scale-110 opacity-100' : 'scale-90 opacity-50'
          "
        >
          <img :src="img" class="max-w-full max-h-full object-contain" />
        </div>
      </div>
      
      <!-- Controls -->
      <div class="flex gap-4">
      
    <button
    @click="next"
    class="px-4 py-2 border rounded hover:bg-gray-100 transition-colors z-10"
    >
    <i class="fa-solid fa-angle-right"></i>
</button>
</div>
</div>  

    <!-- Dots -->
    <div class="flex gap-2 mt-2">
      <span
        v-for="(_, i) in images.length"
        :key="i"
        @click="goTo(i)"
        class="w-3 h-3 rounded-full cursor-pointer transition-colors"
        :class="
          i === currentIndex ? 'bg-blue-600' : 'bg-gray-300 hover:bg-gray-400'
        "
      ></span>
    </div>
<p class="text-[16px]">Мақолаларингиз халқаро даражада тан олинади ва кенг аудиторияга етиб боради</p>

  </div>
</template>

<script setup>
import { ref, computed } from "vue";

const images = [
    "/rectangle/Rectangle 9 (1).png",
    "/rectangle/Rectangle 9 (2).png",
    "/rectangle/Rectangle 9.png",
  "/rectangle/Rectangle 9 (3).png",
  "/rectangle/Rectangle 9 (4).png",
];

const itemWidth = 222; // 206 + margin
const centerIndex = Math.floor(images.length / 2); // Markaziy element indeksi
const currentIndex = ref(centerIndex); // Markazdan boshlash

const translateX = computed(() => {
  // Markaziy elementni ekran markazida ushlab turish
  return (centerIndex - currentIndex.value) * itemWidth;
});

function next() {
  currentIndex.value =
    currentIndex.value < images.length - 1 ? currentIndex.value + 1 : 0;
}

function prev() {
  currentIndex.value =
    currentIndex.value > 0 ? currentIndex.value - 1 : images.length - 1;
}

function goTo(index) {
  currentIndex.value = index;
}
</script>
