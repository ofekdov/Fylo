<template>
    <footer>
        <section class="logo flex column">
            <img src="../assets/imgs/logo.svg" alt=""/>
            <div class="text">
                <div className="icon" v-html="getSvg('locationIcon')"></div>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Incidunt adipisci sunt, temporibus recusandae iure?</p>
            </div>
        </section>
        <section class="content-info flex column">
            <div class="content-way flex align-center">
                <div className="icon" v-html="getSvg('phone')"></div>
                <span>+1-543-123-4567</span>
            </div>
            <div class="content-way flex align-center">
                <div className="icon" v-html="getSvg('email')"></div>
                <span>example@fylo.com</span>
            </div>
        </section>
        <section class="about flex column">
            <span>About Us</span>
            <span>Jobs</span>
            <span>Press</span>
            <span>Blog</span>
        </section>
        <section class="about flex column">
            <span>Content Us</span>
            <span>Terms</span>
            <span>Privacy</span>
        </section>
        <section class="links flex">
            <div class="icon-container">
            <div className="icon" v-html="getSvg('facebook')"></div>
            </div>
            <div class="icon-container">
            <div className="icon" v-html="getSvg('twiter')"></div>
            </div>
            <div class="icon-container">
            <div className="icon" v-html="getSvg('instegram')"></div>
            </div>
        </section>
    </footer>
</template>

<script>
import { svgService } from '../services/svg.service';

export default {
  name: 'AppFooter', 
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
