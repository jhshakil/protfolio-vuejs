<template>
  <div class="bg-gray-100">
    <Navigation></Navigation>
    <HeroSection></HeroSection>
    <AboutMe></AboutMe>
    <MySkill></MySkill>
    <MyProject></MyProject>
    <Footer></Footer>
  </div>
</template>

<script>
import Navigation from "../components/Navigation.vue";
import HeroSection from "@/components/HeroSection.vue";
import AboutMe from "@/components/AboutMe.vue";
import MyProject from "@/components/MyProject.vue";
import MySkill from "@/components/MySkill.vue";
import Footer from "@/components/Footer.vue";
// @ is an alias to /src

export default {
  name: 'HomeView',
  components: {
    Navigation,
    HeroSection,
    AboutMe,
    MyProject,
    MySkill,
    Footer
}
}
</script>
