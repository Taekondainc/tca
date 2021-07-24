<template>
  <div class="flex w-full h-screen items-center justify-center flex-col">
    <form @submit.prevent="submitfaq" class="w-full mt-5">
      <div class="w-full flex items-center justify-center mt-5">
        <h1
          class=" p-10 px-16 rounded-l-sm    bg-gray-50 border-red-600 border-8 border-t-8 border-b-8  "
        >
          Title
        </h1>
        <input
          type="text"
          placeholder="Apple and cherries "
          class="w-3/5 p-10 rounded-l-sm  border-red-600 border-8 border-t-8 border-b-8  "
          v-model="title"
        />
      </div>

      <div class="w-full flex items-center justify-center mt-5">
        <h1
          class=" p-10 rounded-l-sm    bg-gray-50 border-red-600 border-8 border-t-8 border-b-8  "
        >
          Description
        </h1>
        <textarea
          type="text"
          placeholder="Ask Your Questions ???"
          rows="1"
          required
          v-model="question"
          class="w-3/5 p-10 rounded-l-sm  border-red-600 border-8   "
        ></textarea>
      </div>
    <div class="w-full flex items-center justify-center mt-5">  <button
        type="submit"
        class="p-6 border-8 border-red-600 rounded-r-sm  w-3/5  text-gray-50 font-semibold  bg-gray-900"
      >
        Submit
      </button></div>
    </form>
    <div
      class="  text-gray-50 bg-red-600 px-8 py-4 cursor-pointer hover:underline mt-5"
      @click="$router.go(-1)"
    >
      Back
    </div>

    <div
      v-show="hiddenm"
      class="fixed w-full  h-3/4 top-24  left-0 bg-black bg-opacity-90 flex justify-center items-center"
    >
      <div
        v-html="alert"
        class="bg-red-600 text-gray-50 w-full lg:w-1/4 h-2/4 text-2xl text-center flex justify-center items-center p-3"
      ></div>
      <div
        class="absolute right-20 top-0 p-2 border-gray-50  border-2 rounded-full cursor-pointer "
        @click="hout"
      >
        x
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      title: "",
      question: "",
      alert: "",
      hiddenm: false
    };
  },
  methods: {
    submitfaq() {
      axios
        .post("http://localhost:1337/faqs", {
          Question: this.question,
         title: this.title
        })
        .then(res => {
          this.alert = this.res;
          this.question = "";
          this.title = "";

          this.alert =
            "<div>😊😊😊😊😊😊😊</div><div>Your Question was Successfully Sent !!!!!!</div>";
        });
    },

    subscribe() {
      axios
        .post("http://localhost:1337/subscribers", {
          Email: this.email
        })
        .then(res => {
          this.hiddenm = !this.hiddenm;
          this.email = "";
          this.alert =
            "<div>😊😊😊😊😊😊😊</div><div>You are Subscribed  !!!!!!</div>";
        });
    },
    hout() {
      this.hiddenm = !this.hiddenm;
    }
  }
};
</script>

<style lang="scss" scoped>
</style>