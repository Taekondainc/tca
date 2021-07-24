
 <template>
  <!-- This example requires Tailwind CSS v2.0+ -->
  <div class="layout  ">
    <div>
      <nav
        class="fixed w-full top-0 z-20"
        :class="{ change_color: scrollPosition > 100 }"
      >
        <div
          class="max-w-full mx-auto px-6 lg:px-10 flex items-center justify-between h-16 "
          :class="{ cursorh: scrollPosition > 100 }"
        >
          <div class="flex items-center">
            <div class="flex-shrink-0">
              <a href="/">
                <g-image
                  class="h-8 w-8"
                  src="~/assets/logodark.png"
                  alt="Workflow"
              /></a>
            </div>
          </div>

          <div class="flex items-right">
            <div class="flex-shrink-0">
              <div
                class="ml-10 flex items-center space-x-4 lg:space-x-8  text-white text-sm"
                :class="{ cursorpo: scrollPosition > 100 }"
              >
                <a href="/Designs" class="hover:underline">Designs</a>
                <a href="/Branding" class="hover:underline">Branding</a>
                <div @click="menu">
                  <g-image
                    src="~/assets/menu.svg"
                    class="cursor-pointer"
                    :class="{ cursorpo: scrollPosition > 100 }"
                  />
                </div>
              </div>
            </div>
          </div>
        </div>
      </nav>
     <div class="text-3xl text-gray-100 flex flex-col justify-center items-center h-screen   bg-red-600 ">
    <h1>Merchandise Website</h1>    
<h1>Coming soon !!!</h1>
    </div>
    </div>
    <div
      class="max-w-full mx-auto  px-6 lg:p-5    justify-between lg:h-64 bg-white"
    >
      <h1 class=" font-semibold pt-5 lg:pt-0">Taekonda Creative Agency</h1>
      <div
        class="block lg:grid grid-cols-2 w-full items-center justify-items-center   "
      >
        <div
          class="grid grid-cols-2 md:grid-cols-3  lg:grid-cols-3 w-full underline pt-2   "
        >
          <div>
            <div class="pt-1"><a href="/About">About us</a></div>
            <div class="pt-1"><a href="/Blog">Blog</a></div>
            <div class="pt-1"><a href="/Connect">Connect</a></div>
            <div class="pt-1"><a href="/Portfolio">Portfolio</a></div>
          </div>

          <div>
            <div class="pt-1"><a href="/Marketing">Marketing</a></div>
            <div class="pt-1"><a href="/Branding">Branding</a></div>
            <div class="pt-1"><a href="/Design">Design</a></div>
            <div class="pt-1"><a href="/Dev">Web & App Dev</a></div>
          </div>

          <div>
            <div class="pt-1"><a href="/Merchandise">Merchandise</a></div>
            <div class="pt-1"><a href="/Social">Login / Register</a></div>
          </div>
        </div>

        <div
          class="mt-16 lg:mt-0 mb-16 lg:mb-0 lg:grid grid-cols-2 w-full lg:items-center"
        >
          <div class="flex lg:hidden justify-center mb-16 lg:mb-0">
            <a href="# " class="flex items-center "
              ><g-image src="~/assets/upAsset 22.svg" class="w-1/2 mr-0"
            /></a>
          </div>
          <div>
            <h1 class="lg:ml-5 text-center">Download Our App</h1>
            <div class="flex  lg:item-center justify-center   ">
              <g-image src="~/assets/appleAsset 20.svg" class="h-12 ml-5" />
              <g-image src="~/assets/gogle.svg" class="h-12 ml-5" />
            </div>
          </div>
          <div class="hidden lg:flex justify-end  ">
            <a href="# "><g-image src="~/assets/upAsset 22.svg" class="w-1/2"/></a>
          </div>
        </div>
      </div>

      <div class="lg:grid grid-cols-2     items-end pt-5  text-black  ">
        <div
          class="   flex justify-start content-evenly  items-start  w-auto text-black "
        >
          <g-link
            href="https://www.facebook.com/TaekondaINC"
            class="flex items-center"
          >
            <g-image src="~/assets/fb2Asset 24.svg" class="h-4  w-auto mr-3"
          /></g-link>
          <g-link
            href="https://www.instagram.com/taekondainc.592/"
            class="flex items-center"
          >
            <g-image src="~/assets/insta2Asset 25.svg" class="h-4 w-auto mr-3"
          /></g-link>
          <g-link
            href="https://www.behance.net/Taekonda-Inc"
            class="flex items-center"
          >
            <g-image src="~/assets/beh2Asset 26.svg" class="h-4 w-auto mr-3"
          /></g-link>
          <g-link href="mailto:taekondainc@gmail.com" class="flex items-center">
            <g-image src="~/assets/mail2Asset 27.svg" class="h-4 w-auto mr-3"
          /></g-link>
          <div class="hidden lg:block text-xs font-semibold text-black">
            © 2020 TaekondaINC. All Rights Reserved.
          </div>
        </div>

        <div
          class="   lg:flex content-evenly justify-end  w-auto  text-gray-600 pt-5   "
        >
          <g-link
            href="https://www.behance.net/Taekonda-Inc"
            class="lg:ml-4 underline "
          >
            Privacy
          </g-link>
          <g-link href="mailto:taekondainc@gmail.com" class=" ml-4 underline">
            Terms & Conditions</g-link
          >
        </div>
      </div>
    </div>
    <div
      class="fixed w-full h-full  bg-red-600 top-0 z-30 lg:grid grid-cols-2 text-white "
      v-show="show"
    >
      <div class="grid grid-flow-row items-stretch p-10 md:p-20 lg:p-20 text-sm lg:text-lg  h-full relative">
      <button @click="menuclose" class="block  lg:hidden right-2 p-5 text-2xl absolute">  <g-image
                  class=" "
                  src="~/assets/xAsset 3.svg"
                  
                /></button>  <div>
          <div class=" border-b-2 border-white md:w-1/4 lg:w-1/4 mt-10 lg:mt-0">Intro<g-image
                  class="inline float-right"
                  src="~/assets/arrowup.png"
                  height="15px"
                  width="15px"
                /></div>
          <div class="pt-1"><a href="/About">About us</a></div>
          <div class="pt-1"><a href="/Blog">Blog</a></div>
          <div class="pt-1"><a href="/Connect">Connect</a></div>
          <div class="pt-1"><a href="/Portfolio">Portfolio</a></div>
        </div>

        <div>
          <div class=" border-b-2 border-white md:w-1/4 lg:w-1/4">Services<g-image
                  class="inline float-right"
                  src="~/assets/arrowup.png"
                  height="15px"
                  width="15px"
                /></div>
          <div class="pt-1"><a href="/Marketing">Marketing</a></div>
          <div class="pt-1"><a href="/Branding">Branding</a></div>
          <div class="pt-1"><a href="/Design">Design</a></div>
          <div class="pt-1"><a href="/Dev">Web & App Dev</a></div>
        </div>

        <div>
          <div class=" border-b-2 border-white md:w-1/4 lg:w-1/4">Extras<g-image
                  class="inline float-right"
                  src="~/assets/arrowup.png"
                  height="15px"
                  width="15px"
                /></div>
          <div class="pt-1"><a href="/Merchandise">Merchandise</a></div>
          <div class="pt-1"><a href="/Social">Login / Register</a></div>
        </div>
      </div>
      <div class=" bg-black relative hidden md:block lg:block"><button @click="menuclose" class=" right-2 p-5 text-2xl absolute">  <g-image
                  class=" "
                  src="~/assets/xAsset 3.svg"
                  
                /></button>
      <div class="grid items-center  h-full    justify-items-center  "> 
        <g-image
                  class="inline pt-32  self-center"
                  src="~/assets/badgeAsset 2.svg"
                  
                />
                <div class="self-end pb-10">
<a href="">a</a>
<a href="">a</a>
<a href="">a</a>
<a href="">a</a>
<a href="">a</a>
<a href="">a</a>
<a href="">a</a>
<a href="">a</a>

                </div>
        </div></div>
    </div>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>



<script>
export default {
  name: "home",

  data() {
    return {
      call: 100,
      hiden: true,
      show: false,
      scrollPosition: null
    };
  },
  methods: {
    scrolltop() {
      this.hiden = true;
      this.scrollPosition = window.scrollY;
      setTimeout(() => (this.hiden = false), 10000);
    },
    menu() {
      this.show = true;
      console.log(this.show);
    },
    menuclose() {
      this.show = !this.show;
    }
  },
  mounted() {
    window.addEventListener("scroll", this.scrolltop);
  }
};
</script>



<style>
</style>
