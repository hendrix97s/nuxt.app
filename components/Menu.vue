<template>
  <div class="menu h-screen shadow">
    <div class="profile text-center p-2 pb-4 mb-4">
      <img src="~images/03.png" class="rounded-full mb-4 mx-auto polygon" alt="Avatar">
      <h5 class="text-xs mb-1 font-medium leading-tight">Luiz F. Lima</h5>
      <p class="text-gray-500 text-xs">Back-end developer</p>
    </div>

    <div class="buttons">
      <span ><i class="fas fa-apple-alt"></i></span>
    </div>
  </div>
</template>
<style>
@import '~styles/menu.css';  
</style>

<script>
export default {
  name: 'Menu'
}
</script>