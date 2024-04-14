<script setup>
  import HeaderSection from "@/components/HeaderSection.vue";
  import FooterSection from "@/components/FooterSection.vue";
  import IntroSection from "@/components/IntroSection.vue";
  import CarrerSection from "@/components/CarrerSection.vue";
  import PortSection from "@/components/PortSection.vue";
  import ContactSection from "@/components/ContactSection.vue";
  import SkipSection from "@/components/SkipSection.vue";  
</script>

<template>
  <SkipSection />
  <HeaderSection />
  <main id="main" role="main">
    <IntroSection />
    <CarrerSection />
    <PortSection />
    <ContactSection />
  </main>
  <FooterSection />
</template>
