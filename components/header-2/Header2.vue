<template>
  <header class="w-full border-b bg-white">
    <nav class="max-w-[1920px] mx-auto flex items-center justify-between px-6 py-4">

      <!-- LEFT: LOGO -->
      <div class="flex items-center">
        <img src="@/public/Layer1000.png" alt="Logo" class=" w-[165px] h-[70px]">
      </div>

      <!-- CENTER: NAV LINKS -->
      <ul class="flex items-center gap-8 text-[18px] font-medium text-gray-800">
        <li class="flex items-center gap-1 cursor-pointer hover:text-blue-600">
          Журнал ҳақида
          <i class="fa-solid fa-caret-down text-[18px]"></i>
        </li>

        <li class="flex items-center gap-1 cursor-pointer hover:text-blue-600">
          Муаллифлар учун
          <i class="fa-solid fa-caret-down text-[18px]"></i>
        </li>

        <li class="flex items-center gap-1 cursor-pointer hover:text-blue-600">
          Рецензентлар учун
          <i class="fa-solid fa-caret-down text-[18px]"></i>
        </li>

        <li class="cursor-pointer hover:text-blue-600">
          Боғланиш
        </li>
      </ul>

      <!-- RIGHT: ACTIONS -->
      <div class="flex items-center gap-4">

        <!-- Search -->
        <button class="p-2 rounded-md hover:bg-gray-100">
          <i class="fas fa-search"></i>
        </button>

        <!-- Submit article -->
        <button class="flex items-center gap-2 px-4 py-2 bg-[#3861A7] text-white text-sm rounded-md">
        <img
          src="@/public/send.png"
          alt="send"
          class="w-4 h-4"
          style="background: transparent;"
        />

        <span>Мақола юбориш</span>

        </button>

        <!-- User -->
        <img
          src="@/public/human.png"
          alt="user"
          class="w-9 h-9 rounded  cursor-pointer"
        >
      </div>

    </nav>
  </header>
</template>

<script setup>
</script>
