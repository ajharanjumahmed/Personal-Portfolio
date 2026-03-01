<script setup>
import Navbar from './components/layout/Navbar.vue'
import Footer from './components/layout/Footer.vue'

import HeroSection from './components/sections/HeroSection.vue'
import ToolsSection from './components/sections/ToolsSection.vue'
import ServicesSection from './components/sections/ServicesSection.vue'
import ProjectsSection from './components/sections/ProjectsSection.vue'
import StatsSection from './components/sections/StatsSection.vue'
import TestimonialsSection from './components/sections/TestimonialsSection.vue'
import ContactSection from './components/sections/ContactSection.vue'
import LogoShowcase from './components/sections/LogoShowcase.vue'

</script>

<template>
    <Navbar />
    <main>
      <HeroSection/>
      <LogoShowcase/>
      <ToolsSection/>
      <ServicesSection/>
      <ProjectsSection/>
    </main>
</template>

<style scoped>

</style>