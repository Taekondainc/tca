<template>
    <div>
<layout>
    <div class=" h-screen grid grid-rows-2">
<div>
      <div class="pt-20" >    <div class="ttx leading-3 lg:leading-normal ">
                Taekonda Creative Agency
              </div> 
              <div class="  text-lg md:text-2xl lg:text-xl font-semibold
                leading-2 md:leading-tight w-full   lg:w-2/5">
               Seems Like you've Gone Off Course. 
    The Page <span class=" text-yellow-300"> "{{url}}"</span> doesn't Exist. Press the Back Button to Return to your Previous page.
      <div @click="$router.go(-1)" 
      class="px-4 lg:px-12 w-2/5 lg:w-2/5 cursor-pointer focus:ring-offset-purple-500 py-2 my-2
       bg-white text-black  text-base lg:text-xl flex  items-center"> 
             <g-image src="../assets/Icon feather-arrow-up-left.svg" class="ml-3" />Back
          </div></div>
           </div> 
     <div class="  mt-5   flex lg:content-evenly  
          
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
<div class="flex items-center justify-center">
<g-image src="~/assets/404sm.svg" class="block lg:hidden w-4/5
 " />
<g-image src="~/assets/404.svg" class=" 
hidden lg:block  w-5/6" /></div>
    </div>

</layout>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                url:""
            }
        },
        created() {
        var currentUrl = window.location.pathname;
    this.url = currentUrl;
        },
    }
</script>

<style lang="scss" scoped>
</style>