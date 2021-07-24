<template>
  <layout>
    <div>
      <div class=" container   h-screen      ">
        <div
          class=" grid sm:grid-cols-1 lg:grid-cols-2   h-4/5 lg:h-5/6    pt-24 lg:pt-0  "
        >   
          <div class="leading-10  lg:relative z-10 hxhtag">
            <div class="grid items-center   lg:h-full" >
          <div  >    <div class="ttx leading-3 lg:leading-normal ">
                Taekonda Creative Agency
              </div> 
              <div class="textbttm text-3xl md:text-5xl lg:text-5xl font-semibold sm:w-auto leading-8 md:leading-tight  lg:w-full">Connect, <br> Innovate, Explore.</div>
              <div class="mt-1 lg:mt-5">
                <a
                  href="Connect"
                  class="px-3 lg:px-7 py-1 text-xs md:text-xl lg:text-xl inline text-black bg-white lg:leading-2"
                >
                  Connect
                  <g-image
                    class="inline h-4 md:h-4 lg:h-4 w-4 md:w-4 lg:w-4 "
                    src="~/assets/Icon feather-arrow-up-right.svg"
                  />
                </a>
              </div></div>  <div class="hidden lg:block z-0 absolute left-2/4 top-0 lg:top-3">
 <g-image
                    class="w-20  lg:w-40"
                    src="~/assets/Repeat Grid 20.svg"
                  />
            </div>
            </div>

          

          </div>
           <div class="hidden   items-center justify-center    lg:grid  lg:items-end lg:place-items-center my-5 lg:my-0   ">
            <g-image
              src="~/assets/design-edit.svg"
              class="   w-4/6 lg:w-full md:h-5/6   lg:h-5/6   "
            />
          </div>  
          <div class="flex   lg:hidden items-center justify-center  
               lg:items-end lg:place-items-center my-2 lg:my-0     ">
            <g-image
              src="~/assets/pent.svg"
              class="   w-4/6   "
            />
          </div>
        </div>

        <div class="     grid  
         grid-cols-1  lg:grid-cols-2 justify-self-end h-1/6 lg:py-3       ">
          <div
            class=" grid items-end my-5 lg:my-0"
          >
            <p
              class=" w-full   lg:w-3/5 leading-tight  text-base md:text-4xl  lg:text-lg"
            >
              We service Brands & Businesses using the art of design, to grow,
              launch , and build Network in this Connected World.
            </p>
          </div>

          <div class="     flex lg:content-evenly  
          
          place-self-end
           items-end w-full lg:w-auto   lg:pb-1.5  ">
            <g-link
              href="https://www.facebook.com/TaekondaINC"
              class="flex items-center"
            >
              <g-image src="~/assets/fb.svg" class="h-3 md:h-5 lg:h-4  w-auto mr-5"
            /></g-link>
            <g-link
              href="https://www.instagram.com/taekondainc.592/"
              class="flex items-center"
            >
              <g-image src="~/assets/insta.svg" class="h-3 md:h-5 lg:h-4 w-auto mr-5"
            /></g-link>
            <g-link
              href="https://www.behance.net/Taekonda-Inc"
              class="flex items-center"
            >
              <g-image src="~/assets/beh.svg" class="h-3 md:h-5 lg:h-4 w-auto mr-5"
            /></g-link>
            <g-link
              href="mailto:taekondainc@gmail.com"
              class="flex items-center"
            >
              <g-image src="~/assets/mail.svg" class="h-3 md:h-5 lg:h-4 w-auto mr-5"
            /></g-link>
            <div class="tcpy  text-xs md:text-xl lg:text-xs ">
                <span class="block md:hidden lg:hidden">  © 2020 TaekondaINC. </span> 
              <span class="hidden md:block lg:block  ">  © 2020 TaekondaINC. All Rights Reserved.</span> 
            </div>
          </div>
        </div>

        <!--  <div class="grid grid-cols-2     items-center   ">
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
      </div>-->
      </div>
      <div>
        <herosection />
      </div>
    </div>
  </layout>
</template>
<script>
import herosection from "~/components/Herosection";
export default {
  components: {
    herosection,
  },
};
</script>
