<template>
  <section class="Prodactive-content flex align-center justify-center">
    <img src="../assets/imgs/illustration-stay-productive.png" alt=""/>
    <div class="prodactive-text flex column">
        <span class="title">Stay prodactive, wherever you are</span>
        <p>Never let location to be an issue when accessing your files. Fylo has you covered for all of your file storage needs.</p>
        <p>Securely share files and folders with freinds, family and colleagues for live collaboration. No email attachments required.</p>
        <span class="link">See how Fylo works</span>
    </div>
  </section>
</template>

<script>
import { svgService } from '../services/svg.service';
export default {
  name: 'Prodactive', 
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
