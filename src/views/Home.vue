<template>
  <div class="">
    <Header/> 
    <Features/>
    <div class="Pricing"> 
    <Pricing/>
    </div>
    <div class="Team"> 
    <Team/>
    </div>
    <div class="Screen"> 
    <Screen/>
    </div>
    <div class="News"> 
    <News/>
    </div>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from "@/components/Header.vue";
import Features from "@/components/Features.vue";
import Pricing from "@/components/Pricing.vue";
import Team from "@/components/Team.vue";
import Screen from "@/components/Screen.vue";
import News from "@/components/News.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "Home",
  components: {
    Header,
    Features,
    Pricing,
    Team,
    Screen,
    News,
    Footer,
  },
};
import '@/assets/js/scripts.js';
</script>
