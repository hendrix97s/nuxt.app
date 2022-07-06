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
      default: require('assets/images/opengraph.png')
    },
    baseUrl:{
      type: String,
      default: __dirname
    }
  },
  head(){
    return {
      meta: [
        { hid: 'description', name: 'description', content: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s."},
        { hid: 'og:title', property: 'og:title', content: 'Employees - Tests using open graph' },
        { hid: 'og:description', property: 'og:description', content: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s."},
        { hid: 'og:image', property: 'og:image', content: this.image},
        { hid: 'og:type', property: 'og:type', content: 'website' },
        { hid: 'og:site_name', property: 'og:site_name', content: 'Nuxt example with Vercel' },
        { hid: 'og:url', property: 'og:url', content: 'https://nuxt-study.vercel.app/' },
        { hid: 'og:locale', property: 'og:locale', content: 'pt' },

        { hid: 'twitter:title', property: 'twitter:title', content: 'Employees - Tests using open graph' },
        { hid: 'twitter:description', property: 'twitter:description', content: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s."},
        { hid: 'twitter:image', property: 'twitter:image', content: this.image},
        { hid: 'twitter:card', property: 'twitter:card', content: 'summary_large_image'},
        { hid: 'twitter:url', property: 'twitter:url', content: 'https://nuxt-study.vercel.app/'},
      ]
    }
  }
  
})
</script>
