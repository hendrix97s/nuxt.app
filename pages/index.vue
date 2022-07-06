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
  meta: [
    { hid: 'fb:app_id', name: 'fb:app_id', content: '12873892173892' },
    { hid: 'og:title', name: 'og:title', content: 'Teste with OpenGraph' },
    { hid: 'og:image', name: 'og:image', content: '~images/01.png'},
  ],
})
</script>
