<template>
  <section class="details-logos">
    <div class="details">
        <div className="icon" v-html="getSvg('accessAnywhere')"></div>
        <span class="title">Access your files, anywhere</span>
        <p>The ability to use a smartphone, tablet, or computer to access your account means your files follow you everywhere.</p>
    </div>
    <div class="details">
        <div className="icon" v-html="getSvg('security')"></div>
        <span class="title">Security you can trust</span>
        <p>2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files.</p>
    </div>
    <div class="details">
        <div className="icon" v-html="getSvg('collaboration')"></div>
        <span class="title">Real-time collaboration</span>
        <p>securely share files and folders with freinds, family and collegues for live collaboration. No email attachment required.</p>
    </div>
    <div class="details">
        <div className="icon" v-html="getSvg('anyFile')"></div>
        <span class="title">Store any type of file</span>
        <p>Whenever you're sharing holidays photos or work documents, Fylo has you covered allowing for all file types to be securely stored and shared</p>
    </div>
  </section>
</template>

<script>
import { svgService } from '../services/svg.service';
export default {
  name: 'Information', 
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
