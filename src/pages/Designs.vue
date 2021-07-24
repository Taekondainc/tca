<template>
  <layout>
    <div>
    <div class=" justify-center align-middle items-center h-screen      ">
      <div class="grid sm:grid-cols-1 lg:grid-cols-2 justify-items-center  homepx pt-20 lg:pt-0  ">
        <div class="leading-10  grid content-center ">
          <div class="grid  content-end  ">
            <p class="sm:w-auto  lg:w-full leading-tight  text-xs md:text-2xl lg:text-2xl">
              Designs tailored to your marketing strategy. Ensuring that you achieve your goals.

            </p>
            <p class="sm:w-auto  lg:w-full leading-tight  text-xs md:text-2xl lg:text-2xl mt-5  ">Our Design Skills are:<br class="pt-2">
 <a href="#webdesign" class="underline">UX/UI Design</a>,
 <a href="#artdesign" class="underline"> Design</a>,
 <a href="#viddesign" class="underline">Motion Graphics</a>,
 <a href="#design" class="underline">Identity Design</a>,
 <a href="#3ddesign" class="underline"> 3D illustration</a>,
 <a href="#socialdesign" class="underline"> Social Media Design.</a>
 
 
 </p>
            
          </div>
        </div>
        <div class=" flex justify-center   items-center w-full lg:h-full   ">
         
            <g-image src="~/assets/brushAsset 1.svg" class="mb-5 lg:mb-2 lg:pt-10  w-2/6 lg:h-5/6"  />
           
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
      
      <herosectiond/>
    </div>
    
    </div>
  </layout>
</template>
<script>
  import herosectiond from "~/components/HerosectionD" ; 
export default {
  components: {
herosectiond
  }
}
</script>