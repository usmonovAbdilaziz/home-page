<template>
  <div class="w-full flex flex-col items-center h-[624px] bg-[#3861A7]">
    <div class="max-w-[1920px]">
      <!-- CARD -->
      <div class="rounded-2xl flex flex-col items-center">
        <!-- TITLE -->
        <h1 class="text-[48px] mt-[100px] text-white">
          Тошкент Халқаро Университети Илмий онлайн журнали
        </h1>

        <!-- SUBTITLE -->
        <p class="text-[20px] text-[#DBEAFE] mb-8">
          Замонавий тадқиқотлар ва инновацион ғояларингизни дунёга етказинг
        </p>

        <!-- INFO BLOCK -->
        <div
          class="flex bg-transparent border-1 border-[#DBEAFE] bg-white/20 w-[672px] h-[198px] md:flex-row items-center justify-center rounded-[10px] gap-6 mb-8"
        >
          <div class="flex items-center flex-col">
            <!-- LEFT INFO -->
            <div class="flex items-center">
              <div
                class="flex flex-col items-center bg-white/20 pt-2 rounded-[50px] m-3 w-[214px] h-[84px]"
              >
                <p class="text-[14px] text-white m-0">Энг охирги сон</p>
                <p class="text-[30px] text-white m-0">№ 12 (2025)</p>
              </div>

              <div class="h-[70px] w-[2px] bg-white/20 m-2"></div>

              <div class="m-2">
                <p class="text-[14px] text-white m-0">Нашр санаси</p>
                <p class="text-[30px] text-white m-0">Ноябрь 2025</p>
              </div>
            </div>

            <!-- BUTTON -->
            <button
              class="flex items-center justify-center gap-3 px-6 py-3 w-[297px] h-[48px] bg-white text-[#3861A7] rounded-xl"
            >
              <img
                src="@/public/sended2.png"
                alt="send"
                class="w-5 h-5 bg-transparent"
              />
              <span class="font-medium text-[16px]">
                Yagona maqola yuborish
              </span>
            </button>
          </div>
        </div>
      </div>
      <div class="flex items-center gap-6 text-white justify-center">
        <p
          class="w-[283px] h-[102px] border-[1px] border-white/20 bg-white/20 rounded-[10px] flex items-center justify-center flex-col"
        >
          <span class="text-[30px]">500+</span>
          <small class="text-[#DBEAFE]">Нашр этилган мақолалар</small>
        </p>
        <p
          class="w-[283px] h-[102px] border-[1px] border-white/20 bg-white/20 rounded-[10px] flex items-center justify-center flex-col"
        >
          <span class="text-[30px]">200+</span>
          <small class="text-[#DBEAFE]">Муаллифларр</small>
        </p>
        <p
          class="w-[283px] h-[102px] border-[1px] border-white/20 bg-white/20 rounded-[10px] flex items-center justify-center flex-col"
        >
          <span class="text-[30px]">15+</span>
          <small class="text-[#DBEAFE]">Мамлакатлар</small>
        </p>
      </div>
    </div>
  </div>
</template>

<script setup></script>
