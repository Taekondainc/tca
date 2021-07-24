<template>
  <layout>
    <div>
    <div class=" justify-center align-middle items-center h-screen      ">
      <div class="grid sm:grid-cols-1 lg:grid-cols-2 justify-items-center  homepx pt-20 lg:pt-0  ">
        <div class="leading-10  grid content-center ">
          <div class="grid  content-end  ">
            <p class=" lg:w-5/6 leading-tight  text-xs md:text-2xl lg:text-2xl">
            Our full‑stack 
            <span class="underline">Design</span>  and <span class="underline">Development</span>  agency builds strategic user experience, Brand focus and customized Application suited to your business goals and user needs. 
            </p>
           
          </div>
        </div>
        <div class=" flex justify-center w-full items-center   w">
         
            <g-image src="~/assets/dev.svg" class="mb-5 lg:mb-2  w-full lg:w-8/12"  />
           
        </div>
      </div>

      <div class="grid grid-cols-2     items-center   ">
        <div class="   flex justify-start content-evenly  items-start  w-auto ">
          <g-link
            href="https://www.facebook.com/TaekondaINC"
            class="flex items-center"
          >
            <g-image src="~/assets/fb.svg" class="h-4  w-auto mr-3"
          /></g-link>
          <g-link
            href="https://www.instagram.com/taekondainc.592/"
            class="flex items-center"
          >
            <g-image src="~/assets/insta.svg" class="h-4 w-auto mr-3"
          /></g-link>
          <g-link
            href="https://www.behance.net/Taekonda-Inc"
            class="flex items-center"
          >
            <g-image src="~/assets/beh.svg" class="h-4 w-auto mr-3"
          /></g-link>
          <g-link href="mailto:taekondainc@gmail.com" class="flex items-center">
            <g-image src="~/assets/mail.svg" class="h-4 w-auto mr-3"
          /></g-link>
          <div class="hidden lg:block text-xs">© 2020 TaekondaINC. All Rights Reserved.</div>
        </div>

        <div class="   flex content-evenly justify-end  w-auto   ">
          <g-link href="/">
            <g-image src="~/assets/play.png" class="w-10 "
          /></g-link>
        </div>
      </div>
    </div>
    <div>
      
      <herosectiondev />
    </div>
    
    </div>
  </layout>
</template>
<script>
import herosectiondev from "~/components/HerosectionDev" ; 
export default {
  components: {
herosectiondev
  }
}
</script>