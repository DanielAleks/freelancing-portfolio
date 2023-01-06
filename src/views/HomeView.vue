<template>
  <div style="height: 100%; width: 100%">
    <img class="w-full h-full fixed top-0 left-0 object-cover" :src="homeBg" alt="" />
    <div class="w-full h-full fixed top-0 left-0 z-1 overlay"></div>

    <!-- home section - START -->
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

    <div class="w-full flex flex-col justify-center relative z-100" style="height: 100vh">
      <p
        class="text-7xl tracking-wider font-thin w-full text-slate-300 mb-10 mt-10"
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

      <button class="text-slate-300 flex items-center mt-20">
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
    <!-- home section - END -->

    <!-- about section - START -->
    <p class="text-3xl text-gray-300 mt-24 mb-20 w-72">Services I can Provide</p>

    <div class="grid grid-cols-2 gap-x-12 gap-y-20 ml-[3rem] mr-[-3rem] mb-20">
      <div
        v-for="(item, id) in servicesOffered"
        :key="id"
        class="justify-center flex items-center"
      >
        <div class="block p-6 rounded-lg shadow-lg bg-gray-800">
          <h5 class="text-gray-300 text-xl leading-tight font-medium mb-2">
            {{ item.title }}
          </h5>
          <p class="text-gray-400 text-base mb-4">
            {{ item.description }}
          </p>
          <button
            type="button"
            class="inline-block px-6 py-2.5 bg-pink-800 text-white font-medium text-xs leading-tight uppercase rounded shadow-md hover:bg-blue-700 hover:shadow-lg focus:bg-blue-700 focus:shadow-lg focus:outline-none focus:ring-0 active:bg-blue-800 active:shadow-lg transition duration-150 ease-in-out"
          >
            Explore
          </button>
        </div>
      </div>
    </div>
    <!-- about section - END -->

    <!-- contact section - START -->
    <section class="bg-gray-800 dark:bg-gray-900 ml-[3rem] mr-[-3rem] mt-44">
      <div class="py-8 lg:py-16 px-4 mx-auto max-w-screen-md">
        <h2
          class="mb-4 text-4xl tracking-tight font-extrabold text-center text-gray-300 dark:text-white"
        >
          Contact Us
        </h2>
        <p
          class="mb-8 lg:mb-16 font-light text-center text-gray-400 dark:text-gray-400 sm:text-xl"
        >
          Got a technical issue? Want to send feedback about a beta feature? Need details
          about our Business plan? Let us know.
        </p>
        <form action="#" class="space-y-8">
          <div>
            <label
              for="email"
              class="block mb-2 text-sm font-medium text-gray-300 dark:text-gray-300"
              >Your email</label
            >
            <input
              type="email"
              id="email"
              class="shadow-sm bg-gray-800 border border-gray-600 text-gray-900 text-sm rounded-lg focus:ring-primary-500 focus:border-primary-500 block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500 dark:shadow-sm-light"
              placeholder="name@flowbite.com"
              required
            />
          </div>
          <div>
            <label
              for="subject"
              class="block mb-2 text-sm font-medium text-gray-300 dark:text-gray-300"
              >Subject</label
            >
            <input
              type="text"
              id="subject"
              class="block p-3 w-full text-sm bg-gray-800 border-gray-600 text-gray-900 rounded-lg border border-gray-300 shadow-sm focus:ring-primary-500 focus:border-primary-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500 dark:shadow-sm-light"
              placeholder="Let us know how we can help you"
              required
            />
          </div>
          <div class="sm:col-span-2">
            <label
              for="message"
              class="block mb-2 text-sm font-medium text-gray-300 dark:text-gray-400"
              >Your message</label
            >
            <textarea
              id="message"
              rows="6"
              class="block p-2.5 w-full text-sm bg-gray-800 border-gray-600 text-gray-900 rounded-lg shadow-sm border border-gray-300 focus:ring-primary-500 focus:border-primary-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500"
              placeholder="Leave a comment..."
            ></textarea>
          </div>
          <button
            type="submit"
            class="py-3 px-5 text-sm font-medium bg-pink-800 text-center text-white rounded-lg bg-primary-700 sm:w-fit hover:bg-primary-800 focus:ring-4 focus:outline-none focus:ring-primary-300 dark:bg-primary-600 dark:hover:bg-primary-700 dark:focus:ring-primary-800"
          >
            Send message
          </button>
        </form>
      </div>
    </section>
    <!-- contact section - END -->
  </div>
</template>

<style lang="scss">
.overlay {
  background: rgba(0, 0, 0, 0.7);
  backdrop-filter: blur(10px);
}
.card-transparent {
  background: rgba(110, 110, 110, 0.37);
  backdrop-filter: blur(10px);
}
</style>

<script>
import { defineComponent } from "vue";
import homeBg from "../assets/images/homeBg.png";

export default defineComponent({
  setup() {
    const servicesOffered = [
      {
        title: "Front End UI Design",
        description:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      },
      {
        title: "UI UX Development",
        description:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      },
      {
        title: "Website SEO Support",
        description:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      },
      {
        title: "Backend Development with API",
        description:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      },
    ];

    return { homeBg, servicesOffered };
  },
});
</script>
