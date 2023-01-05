<script>
import { defineComponent } from "vue";
import homeBg from "../assets/images/homeBg.png";

export default defineComponent({
  setup() {
    return { homeBg };
  },
});
</script>

<template>
  <div style="height: 100%; width: 100%">
    <img class="w-full h-full fixed top-0 left-0 object-cover" :src="homeBg" alt="" />
    <div class="w-full h-full fixed top-0 left-0 z-1 overlay"></div>

    <div class="nav flex fixed top-14 left-5" style="width: 100%">
      <p class="text-slate-400 absolute left-10 tracking-[.3rem] text-2xl">
        <span style="font-weight: 500">DAN</span
        ><span style="font-weight: 500; opacity: 0.9">IEL </span
        ><span style="font-weight: 400; opacity: 0.8">ALE</span
        ><span style="font-weight: 300; opacity: 0.7">KSA</span
        ><span style="font-weight: 200; opacity: 0.6">NDR</span
        ><span style="font-weight: 100; opacity: 0.6">OV</span>
      </p>
      <div class="absolute right-20 flex items-center">
        <p
          class="text-slate-300 text-lg font-thin border-b h-8 mr-10 leading-tight"
          style="transform: scale(1, 0.9)"
        >
          LET'S TALK
        </p>
        <div class="bg-gray-200 rounded-3xl w-12 h-12 flex items-center justify-center">
          <svg
            class="text-gray-700"
            xmlns="http://www.w3.org/2000/svg"
            width="30"
            height="30"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <line x1="8" y1="12" x2="20" y2="12"></line>
            <line x1="4" y1="6" x2="20" y2="6"></line>
            <line x1="4" y1="18" x2="20" y2="18"></line>
          </svg>
        </div>
      </div>
    </div>

    <div class="w-full h-full relative z-100">
      <p
        class="text-7xl tracking-wider font-thin w-full text-slate-300 mb-10"
        style="width: 65vw"
      >
        <b class="font-semibold">I build</b> intelligent and impactful
        <b>websites</b> that work.
      </p>
      <p class="text-slate-400 text-xl" style="width: 50vw">
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
        incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
        exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      </p>
    </div>

    <button class="text-slate-300 flex items-center mt-5">
      <div class="bg-gray-800 h-12 w-14 rounded-3xl absolute mb-2 ml-1.5"></div>
      <p class="z-1 tracking-widest ml-8 mr-4">SEE MY WORK</p>
      <svg
      class="text-slate-400"
        xmlns="http://www.w3.org/2000/svg"
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        stroke="currentColor"
        stroke-width="2"
        stroke-linecap="round"
        stroke-linejoin="round"
      >
        <polyline points="6 9 12 15 18 9"></polyline>
      </svg>
    </button>
  </div>
</template>

<style lang="scss">
.overlay {
  background: rgba(0, 0, 0, 0.7);
  backdrop-filter: blur(10px);
}
</style>
