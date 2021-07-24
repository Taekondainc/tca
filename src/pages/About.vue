<template>
  <layout>
    <div>
    <div class=" justify-center align-middle items-center h-screen      ">
     
      <div class="block lg:grid    place-content-center  items-center  py-32 md:py-60 lg:py-10">
    <div class="lg:mt-2 text-center text-2xl lg:text-sm mb-5 lg:mb-0">Watch Our video to get briefed on how we aim to serve you.</div>  <video width="1000px" height="200px" controls>
        <source
          src=" "
          type="video/mp4"
          class=" mt-28"
        />
      </video>
      
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
      
      <Herosectiona />
    </div>
    
    </div>
  </layout>
</template>
<script>
import Herosectiona from "~/components/HerosectionA" ; 
export default {
  components: {
Herosectiona
  }
}
</script>
