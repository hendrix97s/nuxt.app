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
        { hid: 'description', name: 'description', content: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book."},
        { hid: 'og:title', property: 'og:title', content: 'Employees - Tests using open graph' },
        { hid: 'og:description', property: 'og:description', content: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book."},
        { hid: 'og:image', property: 'og:image', content: this.image},
        { hid: 'og:image:type', property: 'og:image:type', content: 'image/jpeg'},
        { hid: 'og:image:width', property: 'og:image:width', content: '1200'},
        { hid: 'og:image:height', property: 'og:image:height', content: '630'},
        { hid: 'og:type', property: 'og:type', content: 'website' },
        { hid: 'og:site_name', property: 'og:site_name', content: 'Nuxt example with Vercel' },
        { hid: 'og:url', property: 'og:url', content: 'https://nuxt-study.vercel.app/' },
        { hid: 'og:locale', property: 'og:locale', content: 'pt' },
      ]
    }
  }
  
})
</script>
