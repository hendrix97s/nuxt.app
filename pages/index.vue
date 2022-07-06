<template>
  <div class="container">
    <Menu></Menu>
  </div>
</template>

<style>
@import '~styles/all.scss';
</style>
<script lang="ts">
import Vue from 'vue'
import Test from '~/components/Test.vue'
import Menu from '~/components/Menu.vue'

export default Vue.extend({
  name: "IndexPage",
  components: { Test, Menu },
  props: {
    image: {
      type: String,
      default: require('assets/images/opengraph.jpg')
    },
    baseUrl:{
      type: String,
      default: __dirname
    }
  },
  head(){
    return {
      meta: [
        { hid: 'og-image', property: 'og:image', content: this.image},
        { hid: 'og-url', property: 'og:url', content: 'https://nuxt-study.vercel.app/' },
        { hid: 'og-title', property: 'og:title', content: 'Testes com opengraph' },
        { hid: 'og-desc', property: 'og:description', content: 'This is a sweet post' },
        { hid: 'og-type', property: 'og:type', content: 'website' },
      ]
    }
  }
  
})
</script>
