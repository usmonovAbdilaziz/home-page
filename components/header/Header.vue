<template>
  <header class="w-full bg-[#EEF2F6] border-b">
    <nav class="max-w-[1920px] mx-auto flex flex-row items-center justify-between px-6 py-3">

      <!-- LEFT SIDE -->
      <ul class="flex flex-row items-center gap-6">
        <li class="flex items-center gap-2 text-sm text-gray-700">
          <img src="@/public/emailIcon.png" alt="email" class="w-4 h-4">
          <span>info@tiuglobal.uz</span>
        </li>

        <li class="flex items-center gap-2 text-sm text-gray-700">
          <img src="@/public/phone-flip (1) 1.png" alt="phone" class="w-4 h-4">
          <span>+998 71 244-44-44</span>
        </li>
      </ul>

      <!-- RIGHT SIDE -->
      <div class="relative">
        <button
          @click="toggleDropdown"
          class="flex items-center gap-2 border px-3 py-1.5 rounded-md text-sm hover:bg-gray-100"
        >
          <img src="@/public/flag.png" alt="flag" class="w-4 h-4">
          <span>{{ selectedLang }}</span>
          <span class="text-xs">▼</span>
        </button>

        <!-- DROPDOWN -->
        <ul
          v-show="isOpen"
          class="absolute right-0 mt-2 w-36 bg-white border rounded-md shadow-md"
        >
          <li
            @click="selectLang('Ўзбекча')"
            class="flex items-center gap-2 px-3 py-2 hover:bg-gray-100 cursor-pointer"
          >
            <img src="@/public/flag.png" class="w-4 h-4">
            Ўзбекча
          </li>

          <li
            @click="selectLang('Русский')"
            class="flex items-center gap-2 px-3 py-2 hover:bg-gray-100 cursor-pointer"
          >
            <img src="@/public/flag.png" class="w-4 h-4">
            Русский
          </li>

          <li
            @click="selectLang('English')"
            class="flex items-center gap-2 px-3 py-2 hover:bg-gray-100 cursor-pointer"
          >
            <img src="@/public/flag.png" class="w-4 h-4">
            English
          </li>
        </ul>
      </div>

    </nav>
  </header>
</template>

<script setup>
import { ref } from 'vue'

const isOpen = ref(false)
const selectedLang = ref('Ўзбекча')

const toggleDropdown = () => {
  isOpen.value = !isOpen.value
}

const selectLang = (lang) => {
  selectedLang.value = lang
  isOpen.value = false
}
</script>
