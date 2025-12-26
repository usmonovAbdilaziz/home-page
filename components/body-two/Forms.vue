<template>
  <div class="flex justify-center gap-6 items-start lg:items-stretch w-full max-w-7xl mx-auto px-4 my-24">
<div class="flex flex-col lg:flex-row w-full gap-20">
    <!-- Contact Form -->
    <div class="flex-1 bg-[#F9FAFB] border border-[#E5E7EB] lg:w-[992px] w-[900px] h-[630px] rounded-xl p-6 ">
      <h1 class="text-2xl md:text-3xl font-semibold mb-2">
        Саволларингиз борми?
      </h1>
      <p class="text-base md:text-lg mb-6">
        Саволингиз бизга юборинг, биз кўриб чиқиб сизга алоқага чиқамиз
      </p>

      <form class="flex flex-col gap-5 w-full">
        <!-- FISH -->
        <div class="flex flex-col">
          <label for="fullname" class="text-base md:text-lg">ФИШ:</label>
          <input
            id="fullname"
            type="text"
            placeholder="Киритинг"
            class="w-full px-3 py-2 rounded-xl border border-[#E5E7EB] bg-white"
          />
        </div>

        <!-- Telefon + Email -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-5">
          <div class="flex flex-col">
            <label for="phone" class="text-base md:text-lg">Телефон:</label>
            <input
              id="phone"
              type="tel"
              placeholder="+998"
              class="w-full px-3 py-2 rounded-xl border border-[#E5E7EB] bg-white"
            />
          </div>
          <div class="flex flex-col">
            <label for="email" class="text-base md:text-lg">Email:</label>
            <input
              id="email"
              type="email"
              placeholder="example@email.com"
              class="w-full px-3 py-2 rounded-xl border border-[#E5E7EB] bg-white"
            />
          </div>
        </div>

        <!-- Matn -->
        <div class="flex flex-col">
          <label for="message" class="text-base md:text-lg">Матн:</label>
          <textarea
            id="message"
            rows="4"
            placeholder="Савол мазмуни"
            class="w-full px-3 py-2 rounded-xl border border-[#E5E7EB] bg-white resize-none"
          ></textarea>
        </div>

        <!-- File -->
        <div class="flex flex-col">
          <label for="file" class="text-base md:text-lg">Файл (ихтиёрий):</label>

          <label
            for="file"
            class="flex items-center gap-2 px-4 h-12 border-2 border-dashed border-[#E5E7EB] rounded-xl bg-[#F2F4F8] cursor-pointer text-gray-600 hover:border-[#3861A7] hover:text-[#3861A7] transition"
          >
            <i class="fa-solid fa-file"></i>
            <span>Файл бириктиринг</span>
          </label>

          <input id="file" type="file" class="hidden" />
        </div>

        <!-- Submit -->
        <button
          type="submit"
          class="w-full sm:w-52 h-12 bg-[#3861A7] text-white rounded-xl hover:bg-[#2f4f8f] transition"
        >
          Мурожаатни юбориш
        </button>
      </form>
    </div>
    <!-- Survey -->
    <div class="flex-1 bg-[#F9FAFB] border border-[#E5E7EB] rounded-xl p-6  max-w-md">
      <h2 class="text-xl md:text-2xl font-semibold mb-4">Сўровномалар</h2>

      <form class="bg-white rounded-xl p-4 space-y-3">
        <div>
          <p class="font-medium mb-1">
            Сўровнома! Сайтинг янги дизайнини қандай баҳолайсиз?
          </p>
          <small class="text-gray-500">
            Ушбу сўровнома қатнашиш доирасида бизнинг хизматларини яхшилашда бизга ёрдам берасиз
          </small>
        </div>

        <label class="flex items-center gap-3 p-4 border rounded-xl cursor-pointer">
          <input type="radio" name="survey" value="excellent" class="w-4 h-4 accent-[#3861A7]" />
          <span>Жуда яхши</span>
        </label>

        <label class="flex items-center gap-3 p-4 border rounded-xl cursor-pointer">
          <input type="radio" name="survey" value="good" class="w-4 h-4 accent-[#3861A7]" />
          <span>Яхши</span>
        </label>

        <label class="flex items-center gap-3 p-4 border rounded-xl cursor-pointer">
          <input type="radio" name="survey" value="normal" class="w-4 h-4 accent-[#3861A7]" />
          <span>Қониқарли</span>
        </label>

        <label class="flex items-center gap-3 p-4 border rounded-xl cursor-pointer">
          <input type="radio" name="survey" value="bad" class="w-4 h-4 accent-[#3861A7]" />
          <span>Қониқарсиз</span>
        </label>

        <label class="flex items-center gap-3 p-4 border rounded-xl cursor-pointer">
          <input type="radio" name="survey" value="issues" class="w-4 h-4 accent-[#3861A7]" />
          <span>Камчиликлар мавжуд</span>
        </label>
      </form>

      <button
        class="mt-4 w-full h-12 border border-[#3861A7] text-[#3861A7] rounded-xl hover:bg-[#3861A7] hover:text-white transition"
      >
        Барча сўровномаларни кўриш
      </button>
    </div>
</div>
  </div>
</template>

<script setup></script>
