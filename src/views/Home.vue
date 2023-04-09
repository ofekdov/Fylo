<template>
  <section class="home text-center">
    <img src="../assets/imgs/illustration-intro.png" alt="">
    <h1 class="title">All your files in one secure location,</h1>
    <h1 class="title">accessible anywhere</h1>
    <p>Fylo stores all your most important files in one secure location Access them wherever you need, share and collaborate with freinds family, and co-workers</p>
    <button class="start-btn">Get started</button>
    <div class="curv" className="icon" v-html="getSvg('desktopCurv')"></div>
  </section>
  <section class="information">
    <Information/>
  </section>
  <section class="prodactive">
    <Prodactive/>
  </section>
  <section class="reviews">
    <Reviews/>
  </section>
  <section class="getStarted">
    <GetStarted/>
  </section>
  
  
</template>

<script>
import { svgService } from '../services/svg.service';
import Information from '../cmps/Information.vue'
import Prodactive from '../cmps/Prodactive.vue'
import Reviews from '../cmps/Reviews.vue';
import GetStarted from '../cmps/GetStarted.vue';
export default {
  name: 'home',
  data() {
    return {
    }
  },
  computed: {
  },
  created() {
  },
  methods: {
    getSvg(iconName) {
    return svgService.getSvg(iconName)
  }
  },
  components: {
    Information,
    Prodactive,
    Reviews,
    GetStarted
  }
  
}
</script>
