<template>
  <div class="flex w-full h-full ">
    <Menu></Menu>
    <Schedule></Schedule>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Test from '~/components/Test.vue'
import Menu from '~/components/Menu.vue'
import Schedule from '~/components/Schedule.vue'

export default Vue.extend({
  name: "SchedulePage",
  components: { Test, Menu, Schedule}
})
</script>