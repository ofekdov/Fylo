<template>

<section class="reviews-msgs flex justify-center align-center">
    <div class="review">
        <img class="quotes" src="../assets/imgs/bg-quotes.png" alt="">
        <p>Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.</p>
        <div class="profile flex align-center justify-center">
        <img class="profile-img" src="../assets/imgs/profile-1.jpg" alt="">
        <div class="profile-info flex column align-center">
            <span class="name">Satish patel</span>
            <span class="job">Founder & CEO, Huddle</span>
        </div>
        </div>
    </div>
    <div class="review">
        <p>Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.</p>
        <div class="profile flex align-center justify-center">
        <img class="profile-img" src="../assets/imgs/profile-2.jpg" alt="">
        <div class="profile-info flex column align-center">
            <span class="name">Bruce McKenzie</span>
            <span class="job">Founder & CEO, Huddle</span>
        </div>
        </div>
    </div>
    <div class="review">
        <p>Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.</p>
        <div class="profile flex align-center justify-center">
        <img class="profile-img" src="../assets/imgs/profile-3.jpg" alt="">
        <div class="profile-info flex column align-center">
            <span class="name">Iva Boyd</span>
            <span class="job">Founder & CEO, Huddle</span>
        </div>
        </div>
    </div>
</section>
</template>

<script>
import { svgService } from '../services/svg.service';

export default {
  name: 'Reviews', 
  props: [],
components:{},
created() {},
  data() {
    return {}
  },
  methods: {
    getSvg(iconName) {
    return svgService.getSvg(iconName)
  }
  },
  computed: {},
}

</script>
