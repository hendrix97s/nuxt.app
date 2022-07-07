<template>
    <div class="container-card w-full h-screen flex items-center justify-center">
        <div class="card bg-gradient-to-r flex flex-col items-center justify-center rounded-2xl bg-color-white shadow-2xl">
            <div class="h-full flex">
                <div class="flex flex-col justify-center items-center sm:w-full bg-color-black card-employee-top rounded-2xl ">
                    <img src="https://buzzvel.com/storage/images/logo-light.svg" class="card-img-buzzvel mt-6" alt="buzzvel">
                    <img tabindex="0" class="mt-6 w-3/5 focus:outline-none polygon" src="~images/employees/junior.jpeg" alt="man avatar">
                    <div class="text-center card-emoji polygon bg-white text-gray-900">
                        <span class="card-img-emoji">&#128521;</span>
                        <!-- <img tabindex="0" class="focus:outline-none " src="" alt="man avatar" /> -->
                    </div>
                    <p tabindex="0" class="focus:outline-none mt-5 text-xl font-bold text-center text-white name">Junior Silva</p>
                    <p tabindex="0" class="focus:outline-none mt-2 text-xs  font-light text-center text-white office">Full-stack Developer</p>
                </div>
            </div>
            <div class="flex flex-col justify-center items-center  mt-0">
                <img src="~icons/buzzvel/logo-buzzvel.svg" class="mb-4 icon-buzzvel" alt="buzzvel">
                <!-- <div class="px-10 py-0">
                    <p tabindex="0" class="focus:outline-none mt-0 text-center text-gray-900">
                        Lorem ipsum is simply dummy<br>text of the printing and<br>typesetting industry.
                    </p>
                </div> -->
            </div>
            <div class="mt-0 mb-4 flex flex-col justify-center items-center">
                <img tabindex="0" class="qrcode" src="~images/employees/qrcode/junior-silva.png" alt="man avatar">
                <!-- <img src="~icons/buzzvel/logo-buzzvel.svg" class="w-8 mt-2" alt="buzzvel"> -->
                <p tabindex="0" class="focus:outline-none text-center font-bold  text-gray-900">
                    #ABuzzWayofLife &#128521;
                </p>
            </div>
        </div>

    </div>

</template>
<style>
@import '~styles/all.scss';
@import '~styles/card.css';
</style>
<script lang="ts">
import Vue from 'vue'

export default Vue.extend({

})
</script>