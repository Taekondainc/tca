<template>
  <layout>
    <div>
    <div class=" justify-center align-middle items-center h-screen      ">
      <div class="grid sm:grid-cols-1 lg:grid-cols-2 justify-items-center  homepx pt-20 lg:pt-0  ">
        <div class="leading-10  grid content-center ">
          <div class="grid  content-end  ">
            <p class="sm:w-auto  lg:w-5/6 leading-tight  text-xs md:text-2xl lg:text-2xl">
      Here we feature our latest clients. All the work here combines to create our <span class="underline">Portfolio.</span> 

 
 </p>
            
          </div>
        </div>
        <div class=" flex justify-center w-full items-center   ">
         
            <g-image src="~/assets/portfolio.svg" class="mb-5 lg:mb-2 pt-10  w-full  lg:w-4/6"  />
           
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
      
      <herosectionp />
    </div>
    
    </div>
  </layout>
</template>
<script>
import herosectionp from "~/components/HerosectionP" ; 
export default {
  components: {
herosectionp
  }
}
</script>