<template>
  <div class="alpha">
    <hero-section/>
    <home-section4/>
    <retirement-planning/>
    <home-section2/>
    <features-part/>
    <blog-table/>
    <get-started/>
    <home-section7/>
    <home-section8/>
    <ready-to-work/>
    <footer-home/>
  </div>
</template>

<script>

import HeroSection from "@/components/Home/HeroSection.vue";
import HomeSection4 from "@/components/Home/HomeSection4.vue";
import RetirementPlanning from "@/components/Home/RetirementPlanning.vue";
import HomeSection2 from "@/components/Home/HomeSection2.vue";
import FeaturesPart from "@/components/Home/FeaturesPart.vue";
import BlogTable from "@/components/BaseComponents/tables/BlogTable.vue";
import GetStarted from "@/components/Home/GetStarted.vue";
import HomeSection7 from "@/components/Home/HomeSection7.vue";
import HomeSection8 from "@/components/Home/HomeSection8.vue";
import ReadyToWork from "@/components/Home/ReadyToWork.vue";
import FooterHome from "@/components/BaseComponents/FooterHome.vue";

export default {
  name: 'HomeView',
  components: {
    FooterHome,
    ReadyToWork,
    HomeSection8,
    HomeSection7,
    GetStarted, BlogTable, FeaturesPart, HomeSection2, RetirementPlanning, HomeSection4, HeroSection},
}
</script>
