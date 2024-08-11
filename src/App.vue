<script setup>
import HeroSection from '@/components/HeroSection.vue'
import SectionTwo from '@/components/SectionTwo.vue'
import SectionThree from '@/components/SectionThree.vue'
import SectionFour from '@/components/SectionFour.vue'
import SectionFive from '@/components/SectionFive.vue'
import SectionSix from '@/components/SectionSix.vue'
import SectionSeven from '@/components/SectionSeven.vue'
import SectionEight from '@/components/SectionEight.vue'
import SectionNine from '@/components/SectionNine.vue'
import SectionTen from '@/components/SectionTen.vue'
import Footer from '@/components/Footer.vue'
</script>

<template>
  

  <main>
    <HeroSection />
    <SectionTwo />
    <SectionThree />
    <SectionFour />
    <SectionFive />
    <SectionSix />
    <SectionSeven />
    <SectionEight />
    <SectionNine />
    <SectionTen />
    <Footer />
  </main>
</template>

<style scoped>
/* Prevent horizontal scrolling */
body, html {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}

/* Ensure the width of the content fits the screen */
.container {
  max-width: 100%;
  overflow-x: hidden;
  box-sizing: border-box;
}

/* Apply this globally if needed */
* {
  box-sizing: border-box;
}



</style>