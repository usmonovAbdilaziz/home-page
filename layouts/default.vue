<template>
  <div>
    <Header />
    <Header2 />
    <Dashboard />
    <div class="container">
      <slot />
    </div>
    <Three/>
    <div class="container">
      <One/>
      <Forms/>
    </div>
    <Footer1/>
    <Footer/>
  </div>
</template>

<script setup>
import Header from '~/components/header/Header.vue'
import Footer from '~/components/footer/Footer.vue'
import Header2 from '~/components/header-2/Header2.vue'
import Dashboard from '~/components/dashboard/Dashboard.vue'
import Three from '~/components/body/pages/pages-three/Three.vue'
import One from '~/components/body-two/One.vue'
import Forms from '~/components/body-two/Forms.vue'
import Footer1 from '~/components/body-two/Footer.vue'
</script>

<style src="./default.css"></style>

