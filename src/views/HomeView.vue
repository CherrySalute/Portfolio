<script setup>
  import HeaderSection from "@/components/HeaderSection.vue";
  import FooterSection from "@/components/FooterSection.vue";
  import IntroSection from "@/components/IntroSection.vue";
  import SelfSection from "@/components/SelfSection.vue";
  import CareerSection from "@/components/CareerSection.vue";
  import PortSection from "@/components/PortSection.vue";
  import ContactSection from "@/components/ContactSection.vue";
  import SkipSection from "@/components/SkipSection.vue";  
</script>

<template>
  <SkipSection />
  <HeaderSection />
  <main id="main" role="main">
    <IntroSection />
    <SelfSection />
    <CareerSection />
    <PortSection />
    <ContactSection />
  </main>
  <FooterSection />
</template>
