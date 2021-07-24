<template>
  <div class=" ">
  <div class="py-32">
      <div>
        <h1 class="text-2xl lg:text-7xl font-bold  w-full">
          Let's Design.
          <div>Connect with us to help you achieve your goals.</div>
        </h1>
      
      </div>  <div class="  lg:text-xl py-5">Convinced we're the one for you ??? <div></div>
Connect with us to begin your journey !!! 😊</div>

<div class=" lg:grid grid-cols-2 pt-12 ">
    <form class="w-full lg:w-5/6  " @submit.prevent="messageus">
       <div class="font-semibold text-gray-100">Name</div>
        <input type="text" class=" bg-transparent border-b-2 p-2 mb-8 w-full lg:w-3/4 focus:outline-none" v-model="name" placeholder="Mercy Jones" required>
     <div class="font-semibold text-gray-100">Contact Info</div> 
       <input type="text" class=" bg-transparent border-b-2 p-2 mb-8 w-full lg:w-3/4 focus:outline-none" v-model="contact" placeholder="Email or Phone Number" required>
      <Div class="font-semibold text-gray-100 ">Description</Div> 
      <div class="lg:flex flex-wrap content-end  "> 
          <textarea type="text" class=" bg-transparent border-b-2 p-2 mb-7 lg:mb-0 focus:outline-none w-full lg:w-3/4"  v-model="description" 
        placeholder="Consult us on Anything you need.😊 " required></textarea>
        <div class="lg:hidden "></div>
    
         <button class=" lg:inline lg:ml-6 self-end
         h-2/4 cursor-pointer hover:bg-red-600 " type="submit">    <g-image src="~/assets/submit.svg"   /></button>
         </div>
       <div   v-show="hiddenm" class="fixed w-full  h-3/4 top-24  left-0 bg-black bg-opacity-90 flex justify-center items-center">
         <div v-html="alert" class="bg-red-600 text-gray-50 w-full lg:w-1/4 h-2/4 text-2xl text-center flex justify-center items-center p-3"></div>
         <div class="absolute right-20 top-0 p-2 border-gray-50  border-2 rounded-full cursor-pointer " @click="hout">x</div>
       </div>
       <div  ></div>
    </form> 
    <div class="flex justify-center">
        <g-image src="~/assets/prob.svg" class="hidden lg:block w-2/5" />
    </div>
</div>

    </div>

    <div class="flex md:grid lg:grid    flex-col-reverse md:grid-cols-2 lg:grid-cols-2 place-content-center 
     items-center py-20 lg:py-32   lg:px-16">
      <div class=" ">
        <h1 class="text-3xl lg:text-6xl font-bold pb-5">Office Hours:</h1>
        <div class="lg:w-5/6  text-lg lg:text-2xl  ">
          <ul>
            <li>Monday: 10:15 AM - 6:00 PM</li>
            <li>Tuesday: 10:15 AM - 6:00 PM</li>
            <li>Wednesday: 10:15 AM - 6:00 PM</li>
            <li>Thursday: 10:15 AM - 6:00 PM</li>
            <li>Friday: 10:15 AM - 6:00 PM</li>
            <li>Saturday: 10:15 AM - 6:00 PM</li>
          </ul>
        </div>
      </div>
      <div class="flex items-center justify-center order-1 lg:order-2 w-full mb-7 lg:mb-0">
        <g-image src="~/assets/openinghAsset 18.svg" class="lg:w-4/6" />
      </div>
    </div>
 <div class="py-32">
      <iframe
        class="w-full"
        id="maps"
        height="500px"
        src="https://maps.google.com/maps?q=lot 2 Mandela Avenue,Georgetown,Guyana&output=embed"
      ></iframe>
    </div>
    <div>
      <div class="text-center w-full py-32">
        <div class="text-center w-full flex justify-center py-3 mb-7 lg:mb-14">
          <g-image src="~/assets/socialAsset 19.svg" />
        </div>
        <h1 class="pt text-2xl lg:text-5xl   mt-5  text-center font-bold">
          Our Socials for you to connect with us.
        </h1>
        <div class="grid grid-cols-4 mt-10 lg:mt-16">
          <div class="flip0 ">
            <a href="#maps" class=" flex">
              <g-image
                src="~/assets/locationAsset 20.svg"
                alt=""
                class="w-full "
              />
            </a>
            <a href="https://www.behance.net/Taekonda-Inc" class="flex"
              ><g-image src="~/assets/behanceAsset 21.svg" alt="" class="w-full" />
            </a>
          </div>

          <div>
            <a href="https://www.facebook.com/TaekondaINC" class="flex"
              ><g-image src="~/assets/fbAsset 22.svg" alt="" class="w-full" />
            </a>
            <a href="https://dribbble.com/TaekondaInc" class="flex"
              ><g-image src="~/assets/dribbleAsset 23.svg" alt="" class="w-full" />
            </a>
            <a href="tel:+592-616-1446" class="flex"
              ><g-image src="~/assets/callAsset 24.svg" alt="" class="w-full" />
            </a>
          </div>

          <div>
            <a href="https://www.instagram.com/taekondainc.592/" class="flex"
              ><g-image
                src="~/assets/instaAsset 25.svg"
                alt=""
                class="w-full"
              /> </a
            ><a
              href="https://www.linkedin.com/company/taekonda-creative-agency"
              class="flex"
              ><g-image src="~/assets/linknAsset 26.svg" alt="" class="w-full" />
            </a>
            <a href="mailto:+taekondainc@gmail.com" class="flex"
              ><g-image src="~/assets/mailAsset 27.svg" alt="" class="w-full" />
            </a>
          </div>

          <div>
            <a href="https://www.pinterest.com/TCA592" class="flex"
              ><g-image
                src="~/assets/pinterestAsset 29.svg"
                alt=""
                class="w-full"
              />
            </a>

            <a href="http://github.com/Taekondainc." class="flex"
              ><g-image src="~/assets/githubAsset 28.svg" alt="" class="w-full" />
            </a>
          </div>
        </div>
      </div>
    </div>

    <div class="block lg:grid grid-cols-2  place-content-center  items-center pt-24 mb-16 lg:mb-0  ">
      <div>
        <h1 class=" text-3xl lg:text-6xl font-bold pb-5">Subscribe</h1>
        <div class="lg:w-10/12">
       Trust us we wont spam you with useless promotions. Our Daily newsletter is only filled with articles that will help you better your ROI and comany.
       <div class="flex content-around pt-4 w-full ">
            <form @submit.prevent="subscribe" class="w-full"> 
            <input type="email" placeholder="Email" pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,}$" 
             v-model="email"  class="h-9 w-3/6 text-black placeholder-gray-600 font-semibold p-2" required   />
        <button type="submit" class="p-0 m-0 h-full focus:outline-none focus:ring-4 focus:ring-yellow-800  ">
          <g-image src="~/assets/submitAsset 19.svg" class="h-9 btndiv   inline p-0 cursor-pointer
            outline-none "  /> </button> </form>  
          </div>
        </div>
      </div>
      <div class="hidden lg:flex items-center justify-end h-32 lg:h-3/4 w-full    ">
        <g-image src="~/assets/george-pagan-iii-FBwW4Xu3FTs-unsplash.jpg" class="mt-10 lg:mt-0 w-full lg:w-5/6 h-1/6 lg:h-5/6
        object-contain  lg:object-cover bg-blend-overlay" />
      </div>
    </div>

  
  </div>
</template>

<script>
import axios from 'axios';
export default {
  data() {
    return {
      name:"",
      contact:"",
      description:"",
      alert:"",
      hiddenm:false,
email:""
    }
  },
  methods: {
    messageus(){
axios.post("http://localhost:1337/messages",{
  "Name":this.name,
  "Contact":this.contact,
  "Description":this.description
}).then(res=>{this.alert=this.res;
this.name="";
this.contact="";
this.description="";
this.hiddenm =!this.hiddenm;
 this.alert="<div>😊😊😊😊😊😊😊</div><div>Your Message was Successfully Sent !!!!!!</div>" ;
});
    },
 
    subscribe(){
axios.post("http://localhost:1337/subscribers",{
  "Email":this.email,
   
}).then(res=>{ 
this.hiddenm =!this.hiddenm;this.email="";
 this.alert="<div>😊😊😊😊😊😊😊</div><div>You are Subscribed  !!!!!!</div>" ;
});
    },
    hout(){
      this.hiddenm =!this.hiddenm;
    }
  },
};
</script>

<style lang="scss" scoped>
</style>