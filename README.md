# TIU Global Tadqiqotlar va Innovatsiyalar Ilmiy Jurnali

Ushbu loyiha **TIU Global** tadqiqotlar va innovatsiyalar ilmiy jurnali uchun zamonaviy va interaktiv veb-saytning frontend qismidir. Loyiha **Nuxt 3** (Nuxt 4 framework asosida) va **Tailwind CSS** yordamida qilingan.

## 🚀 Texnologiyalar stacki

- **Framework:** [Nuxt 3/4](https://nuxt.com/)
- **UI & Styling:** [Tailwind CSS](https://tailwindcss.com/)
- **Icons:** FontAwesome
- **Frontend Logic:** Vue 3 (Composition API)

## 📁 Loyiha tuzilmasi

Loyihaning muhim qismlari quyidagilardan iborat:

- `/components`: Barcha vizual komponentlar shu yerda joylashgan.
  - `header/` va `header-2/`: Saytning yuqori qismi (navigatsiya).
  - `body/`: Asosiy HeroSection va boshqa sahifa qismlari.
  - `body-two/`:
    - `One.vue`: Xalqaro indeksatsiya bazalari karuseli.
    - `Forms.vue`: Aloqa formasi va so'rovnomalar.
    - `Footer.vue`: Hamkorlar bo'limi.
  - `footer/`: Saytning asosiy quyi qismi (kontaktdar va havolalar).
- `/layouts`: Sahifaning umumiy tuzilmasi (`default.vue`).
- `/pages`: Saytning marshrutlari (router).
- `/public`: Statik resurslar (rasmlar, ikonka).

## ✨ Asosiy Imkoniyatlar

1.  **Interaktiv Karusel**: Xalqaro indeksatsiya bazalari uchun maxsus tayyorlangan, markazlashtirilgan carousel.
2.  **Aloqa Formasi**: Foydalanuvchilar savol yuborishi va fayl biriktirishi uchun qulay forma.
3.  **So'rovnomalar**: Sayt sifati va dizaynini baholash uchun interaktiv so'rovnoma bo'limi.
4.  **Moslashuvchan Dizayn (Responsive)**: Sayt mobil qurilmalar, planshetlar va desktop ekranlarga to'liq moslashgan.

## 🛠 O'rnatish va Ishga tushirish

Loyihani mahalliy xotirada ishga tushirish uchun quyidagi qadamlarni bajaring:

1.  **Bog'liqliklarni o'rnatish:**

    ```bash
    pnpm install
    ```

2.  **Development rejimida ishga tushirish:**

    ```bash
    pnpm run dev
    ```

3.  **Production build yaratish:**
    ```bash
    pnpm run build
    ```
---

© 2024 TIU Global tadqiqotlar va innovatsiyalar ilmiy jurnali. Барча ҳуқуқлар ҳимояланган.
