<template>
  <div class="w-full">
    <slide-y-down-transition>
      <nuxt-link
        v-if="isVisible"
        to="./"
        @click.native="scrollUp"
        class="w-10 h-10 bg-gray-800 hover:bg-opacity-75 text-gray-200 hover:text-opacity-75 transition-all duration-300 ease-in-out rounded-full flex flex-wrap justify-center items-center fixed bottom-0 right-0 mr-10 lg:mr-24 mb-10 focus:outline-none focus:ring-2 ring-blue-500 z-20"
      >
        <svg class="w-5 fill-current" viewBox="0 0 24 24"><path d="M11.2929 8.2929c.3905-.3905 1.0237-.3905 1.4142 0l6 6c.3905.3905.3905 1.0237 0 1.4142-.3905.3905-1.0237.3905-1.4142 0L12 10.4142l-5.2929 5.2929c-.3905.3905-1.0237.3905-1.4142 0-.3905-.3905-.3905-1.0237 0-1.4142l6-6z" /></svg>
      </nuxt-link>
    </slide-y-down-transition>
    <div class="w-full flex flex-wrap items-center justify-start bg-gray-200 clip-path-1 relative">
      <div class="container mx-auto pt-32 pb-24">
        <div class="w-full flex flex-wrap items-start justify-center content-center">
          <div class="px-5 py-5 mx-0 md:mx-6 flex flex-wrap flex-col items-center content-center md:content-start justify-center md:justify-start">
            <h1 style='font-weight: bold; font-size: 24px'>Hamdan Ali Baloch</h1>
            <div class="space-x-0 md:space-x-7 w-full max-w-1/2 md:max-w-full flex flex-wrap flex-row items-center content-center md:content-start justify-center md:justify-start mt-8">
              <nuxt-link to="/" class="nav-links-footer">Home</nuxt-link>
              <nuxt-link to="#services" class="nav-links-footer">Services</nuxt-link>
              <nuxt-link to="#about" class="nav-links-footer">About</nuxt-link>
              <nuxt-link to="#experience" class="nav-links-footer">Experience</nuxt-link>
              <nuxt-link to="#contact" class="nav-links-footer">Contact</nuxt-link>
              <nuxt-link to="/apps/" class="nav-links-footer">Projects</nuxt-link>
            </div>
          </div>
          <div class="w-full px-5 py-5 flex flex-wrap items-center justify-center">
            <subscription-form></subscription-form>
          </div>
          <div class="w-full text-center absolute bottom-0 py-3 px-6 md:px-52 flex flex-wrap justify-between items-center">
            <span class="text-base text-gray-600 ">Copyright 2022 - Hamdan Ali Baloch</span>
            <div class="flex flex-wrap items-center justify-center">
              <a href="https://github.com/hamdan3555" target="_blank" class="text-gray-600 hover:text-opacity-70 hover:-translate-y-1 transform p-1 rounded-full transition-all duration-300 ease-out">
                <svg class="fill-current w-5 h-5" viewBox="0 0 24 24"><path d="M16 23c-.6 0-1-.4-1-1v-3.9c.1-.8-.2-1.4-.7-1.9-.3-.3-.4-.7-.2-1 .1-.4.5-.6.8-.7 2.9-.3 5.6-1.3 5.6-6 0-1.1-.4-2.2-1.2-3.1-.3-.3-.3-.7-.2-1 .3-.8.3-1.6.1-2.4-.5.1-1.3.4-2.6 1.3-.2.2-.5.2-.8.1-2.1-.6-4.4-.6-6.5 0-.3.1-.6.1-.9-.1C7.2 2.4 6.3 2.1 5.8 2c-.2.8-.2 1.6.1 2.4.1.4.1.8-.2 1-.8.9-1.2 2-1.2 3.1 0 4.7 2.7 5.7 5.6 6 .4 0 .7.3.8.7.1.4 0 .8-.2 1-.5.5-.7 1.1-.7 1.8v3.9c0 .6-.4 1-1 1s-1-.4-1-1v-1.7c-3 .5-4.3-1.2-5.2-2.3-.4-.5-.7-.9-1.1-1-.5-.1-.9-.7-.7-1.2.1-.5.7-.9 1.2-.7 1 .3 1.6 1 2.2 1.7.8 1.1 1.5 1.9 3.6 1.5v-.1c0-.6.1-1.3.3-1.8-2.8-.6-5.8-2.4-5.8-7.7 0-1.5.5-2.9 1.4-4-.4-1.4-.3-2.7.3-4 .1-.3.3-.5.6-.6.4-.1 1.7-.3 4.4 1.4 2.2-.5 4.5-.5 6.6 0 2.6-1.7 4-1.5 4.4-1.4.3.1.5.3.6.6.5 1.3.6 2.6.3 3.9.9 1.1 1.4 2.5 1.4 4 0 5.7-3.4 7.2-5.8 7.8.2.6.3 1.3.3 1.9V22c0 .6-.4 1-1 1z" /><defs><clipPath id="clip0"><path d="M0 0h24v24H0V0z"/></clipPath></defs></svg>
              </a>
              <a href="https://www.linkedin.com/in/hamdan-ali-baloch-551952197/" target="_blank" class="text-gray-600 hover:text-opacity-70 hover:-translate-y-1 transform p-1 rounded-full transition-all duration-300 ease-out">
                <svg class="fill-current w-5 h-5" viewBox="0 0 24 24"><path fill-rule="evenodd" clip-rule="evenodd" d="M16 9a4.9997 4.9997 0 00-5 5v6h2v-6a3 3 0 016 0v6h2v-6a4.9997 4.9997 0 00-5-5zm0-2a6.9998 6.9998 0 00-7 7v7c0 .5523.4477 1 1 1h4c.5523 0 1-.4477 1-1v-7a1.0001 1.0001 0 012 0v7c0 .5523.4477 1 1 1h4c.5523 0 1-.4477 1-1v-7a6.9999 6.9999 0 00-7-7zM1 9c0-.5523.4477-1 1-1h4c.5523 0 1 .4477 1 1v12c0 .5523-.4477 1-1 1H2c-.5523 0-1-.4477-1-1V9zm2 1v10h2V10H3zM4 3c-.5523 0-1 .4477-1 1s.4477 1 1 1 1-.4477 1-1-.4477-1-1-1zM1 4c0-1.6568 1.3432-3 3-3 1.6569 0 3 1.3432 3 3 0 1.6569-1.3431 3-3 3-1.6568 0-3-1.3431-3-3z"/></svg>
              </a>
              <a href="https://www.instagram.com/hamdan_ali_baloch/" target="_blank" class="text-gray-600 hover:text-opacity-70 hover:-translate-y-1 transform p-1 rounded-full transition-all duration-300 ease-out">
                <svg class="fill-current w-5 h-5" viewBox="0 0 24 24"><path fill-rule="evenodd" clip-rule="evenodd" d="M7 3C4.7909 3 3 4.7909 3 7v10c0 2.2091 1.7909 4 4 4h10c2.2091 0 4-1.7909 4-4V7c0-2.2091-1.7909-4-4-4H7zM1 7c0-3.3137 2.6863-6 6-6h10c3.3137 0 6 2.6863 6 6v10c0 3.3137-2.6863 6-6 6H7c-3.3137 0-6-2.6863-6-6V7z" /><path fill-rule="evenodd" clip-rule="evenodd" d="M12.4833 8.9892a2.9998 2.9998 0 00-3.402 3.4441 3.0002 3.0002 0 002.4854 2.4853 2.9996 2.9996 0 003.4441-3.4019 3 3 0 00-2.5275-2.5275zM9.7404 7.5186a5 5 0 114.6058 8.8764 5 5 0 01-4.6058-8.8764z" /></svg>
              </a>
              <a href="https://api.whatsapp.com/send?phone=923166783632&text=Hello%20this%20is%20the%20starting%20message" target="_blank" class="text-gray-600 hover:text-opacity-70 hover:-translate-y-1 transform p-1 rounded-full transition-all duration-300 ease-out">
                <svg width="20px" height="20px" viewBox="0 0 24 24" role="img" xmlns="http://www.w3.org/2000/svg"><title>WhatsApp icon</title><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413Z"/></svg>              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { SlideYDownTransition } from "vue2-transitions";
import SubscriptionForm from "@/components/library/SubscriptionForm";

export default {
  data() {
    return {
      isVisible: false,
      lastScrollPosition: 0,
    };
  },
  methods: {
    scrollUp() {
      // window.scrollTo(0,0);
      window.scrollTo(0, 0, 0, undefined, true);
    },
    handleScroll(e) {
      let scrollPos = window.scrollY;
      // let winHeight = window.innerHeight
      // let docHeight = document.documentElement.scrollHeight

      if (scrollPos > 250) {
        this.isVisible = true;
      } else {
        this.isVisible = false;
      }
    },
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  },
  components: {
    SlideYDownTransition,
    SubscriptionForm,
  },
};
</script>
<style lang="scss">
.clip-path-1 {
  clip-path: polygon(0 15%, 100% 0, 100% 100%, 0% 100%);

  @media (min-width: 768px) {
    clip-path: polygon(0 15%, 100% 0, 100% 100%, 0% 100%);
  }
}
.nav-links-footer {
    @apply items-center text-base px-4 md:px-0 w-1/2 md:w-auto md:text-lg font-medium text-gray-600 hover:text-opacity-70 focus:underline focus:outline-none transition-all duration-300;

    &:nth-child(odd){
      @apply text-right;
    }
}
</style>
