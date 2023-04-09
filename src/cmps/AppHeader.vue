<template>
  <header>
    <div class="logo flex align-center justify-center">
        <div class="flex align-center justify-center" className="icon" v-html="getSvg('logo')"></div>
    </div>
    <nav class="flex align-center justify-center">
      <span class="route-btn">Features</span>
      <span class="route-btn">Team</span>
      <span class="route-btn">Sign in</span>
    </nav>
   
  </header>
</template>
<script>
import { svgService } from '../services/svg.service';
export default {
  name: 'AppHeader', 
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