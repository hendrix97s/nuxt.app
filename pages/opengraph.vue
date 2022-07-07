<template>
<div class="w-full h-screen flex items-center justify-center shadow-2xl">
  <div class="opengraph-container flex items-center justify-center relative shadow-2xl color-black">

    <div class="circle-right-external absolute">
      <div class="circle-right-internal absolute"></div>
    </div>

    <div class="text-box absolute color-black">
      <h2 class="font-light">
        We help you to<br>
        bring your idea or<br>
        product to life
        </h2>

        <div class="flex lg:pr-24">
          <span class="mt-8 text-xl leading-5 let-talk-gradient font-medium mr-5 lg:block">Let's talk</span>
          <img class="cursor-pointer pt-1 mt-4 hover-let-talk" src="~icons/buzzvel/button-let-talk.svg" title="button-let-talk" alt="button-let-talk">
        </div>
    </div>

    <div class="flex items-center justify-center profile text-center polygon">
      <img src="~images/employees/junior.jpeg" class="mx-auto polygon" alt="Avatar">
    </div>

    <div class="absolute emoji flex items-center justify-center profile text-center polygon">
        &#128521;
    </div>

    <div class="name-developer absolute w-full text-center">
        <h5 class="text-gray-100 text-2xl font-bold leading-tight">Junior Silva</h5>
        <p class="text-gray-100 text-2xs font-light">Full-stack developer</p>
    </div>

    <div class="footer absolute inset-x-0 bottom-0 left-0 pl-8"></div>
    <img class="logo-buzzvel absolute" src="~icons/buzzvel/logo-buzzvel-black.svg">
  </div>
</div>
</template>
<style>
@import '~styles/opengraph.css';
@import '~styles/all.scss';
</style>
<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
    props: {
    image: {
      type: String,
      default: require('assets/images/opengraph.jpg')
    },
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
        { hid: 'og:url', property: 'og:url', content: 'https://nuxt-study.vercel.app/opengraph' },
        { hid: 'og:locale', property: 'og:locale', content: 'pt' },

        { hid: 'twitter:title', property: 'twitter:title', content: 'Employees - Tests using open graph' },
        { hid: 'twitter:description', property: 'twitter:description', content: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s."},
        { hid: 'twitter:image', property: 'twitter:image', content: this.image},
        { hid: 'twitter:card', property: 'twitter:card', content: 'summary_large_image'},
        { hid: 'twitter:url', property: 'twitter:url', content: 'https://nuxt-study.vercel.app/opengraph'},
      ]
    }
  }
})
</script>