<script setup>
import { Head, Link } from "@inertiajs/vue3";

defineProps({
    canLogin: Boolean,
    canRegister: Boolean,
    laravelVersion: String,
    phpVersion: String,
});
</script>

<template>
<!-- Main navigation container -->
<nav
  class="flex-no-wrap relative flex w-full items-center justify-between bg-[#FBFBFB] py-2 shadow-md shadow-black/5 dark:bg-black dark:shadow-black/10 lg:flex-wrap lg:justify-start lg:py-4">
  <div class="flex w-full flex-wrap items-center justify-between px-3">
    <!-- Hamburger button for mobile view -->
    <button
      class="block border-0 bg-transparent px-2 text-neutral-500 hover:no-underline hover:shadow-none focus:no-underline focus:shadow-none focus:outline-none focus:ring-0 dark:text-neutral-200 lg:hidden"
      type="button"
      data-te-collapse-init
      data-te-target="#navbarSupportedContent1"
      aria-controls="navbarSupportedContent1"
      aria-expanded="false"
      aria-label="Toggle navigation">
      <!-- Hamburger icon -->
      <span class="[&>svg]:w-7">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 24"
          fill="currentColor"
          class="h-7 w-7">
          <path
            fill-rule="evenodd"
            d="M3 6.75A.75.75 0 013.75 6h16.5a.75.75 0 010 1.5H3.75A.75.75 0 013 6.75zM3 12a.75.75 0 01.75-.75h16.5a.75.75 0 010 1.5H3.75A.75.75 0 013 12zm0 5.25a.75.75 0 01.75-.75h16.5a.75.75 0 010 1.5H3.75a.75.75 0 01-.75-.75z"
            clip-rule="evenodd" />
        </svg>
      </span>
    </button>

    <!-- Collapsible navigation container -->
    <div
      class="!visible hidden flex-grow basis-[100%] items-center lg:!flex lg:basis-auto"
      id="navbarSupportedContent1"
      data-te-collapse-item>
      <!-- Logo -->
      <a
        class="mb-6 ml-2 mr-5 mt-3 flex items-center text-neutral-900 hover:text-neutral-900 focus:text-neutral-900 dark:text-neutral-200 dark:hover:text-neutral-400 dark:focus:text-neutral-400 lg:mb-0 lg:mt-0"
        href="https://yovanenovore.tech">
        <img
          src="https://raw.githubusercontent.com/ynvYauneEnovore/personal-port/main/public/img/ynv.png"
          style="height: 50px"
          alt="TE Logo"
          loading="lazy" />
      </a>
      <!-- Left navigation links -->
      <ul
        class="list-style-none mr-auto flex flex-col pl-0 lg:flex-row"
        data-te-navbar-nav-ref>
        <li class="mb-4 lg:mb-0 lg:pr-2" data-te-nav-item-ref>
          <!-- Dashboard link -->
          <a
            class="text-neutral-500 transition duration-200 hover:text-neutral-700 hover:ease-in-out focus:text-neutral-700 disabled:text-black/30 motion-reduce:transition-none dark:text-neutral-200 dark:hover:text-neutral-300 dark:focus:text-neutral-300 lg:px-2 [&.active]:text-black/90 dark:[&.active]:text-zinc-400 active"
            href="#"
            data-te-nav-link-ref
            >Himnos</a
          >
        </li>
        <!-- Team link -->
        <li class="mb-4 lg:mb-0 lg:pr-2" data-te-nav-item-ref>
          <a
            class="text-neutral-500 transition duration-200 hover:text-neutral-700 hover:ease-in-out focus:text-neutral-700 disabled:text-black/30 motion-reduce:transition-none dark:text-neutral-200 dark:hover:text-neutral-300 dark:focus:text-neutral-300 lg:px-2 [&.active]:text-black/90 dark:[&.active]:text-neutral-400"
            href="#"
            data-te-nav-link-ref
            >Mapas</a
          >
        </li>
        <!-- Projects link -->
        <li class="mb-4 lg:mb-0 lg:pr-2" data-te-nav-item-ref>
          <a
            class="text-neutral-500 transition duration-200 hover:text-neutral-700 hover:ease-in-out focus:text-neutral-700 disabled:text-black/30 motion-reduce:transition-none dark:text-neutral-200 dark:hover:text-neutral-300 dark:focus:text-neutral-300 lg:px-2 [&.active]:text-black/90 dark:[&.active]:text-neutral-400"
            href="#"
            data-te-nav-link-ref
            >Simbolos</a
          >
        </li>
      </ul>
    </div>

    <!-- Right elements -->
    <div class="relative flex items-center">
      <!-- Cart Icon -->
      <a
        class="mr-4 text-neutral-600 transition duration-200 hover:text-neutral-700 hover:ease-in-out focus:text-neutral-700 disabled:text-black/30 motion-reduce:transition-none dark:text-neutral-200 dark:hover:text-neutral-300 dark:focus:text-neutral-300 [&.active]:text-black/90 dark:[&.active]:text-neutral-400"
        href="#">
        <span class="[&>svg]:w-5">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            fill="currentColor"
            class="h-5 w-5">
            <path
              d="M2.25 2.25a.75.75 0 000 1.5h1.386c.17 0 .318.114.362.278l2.558 9.592a3.752 3.752 0 00-2.806 3.63c0 .414.336.75.75.75h15.75a.75.75 0 000-1.5H5.378A2.25 2.25 0 017.5 15h11.218a.75.75 0 00.674-.421 60.358 60.358 0 002.96-7.228.75.75 0 00-.525-.965A60.864 60.864 0 005.68 4.509l-.232-.867A1.875 1.875 0 003.636 2.25H2.25zM3.75 20.25a1.5 1.5 0 113 0 1.5 1.5 0 01-3 0zM16.5 20.25a1.5 1.5 0 113 0 1.5 1.5 0 01-3 0z" />
          </svg>
        </span>
      </a>

      <!-- Container with two dropdown menus -->
      <div
        class="relative"
        data-te-dropdown-ref
        data-te-dropdown-alignment="end">
        <!-- First dropdown trigger -->
        <a
          class="hidden-arrow mr-4 flex items-center text-neutral-600 transition duration-200 hover:text-neutral-700 hover:ease-in-out focus:text-neutral-700 disabled:text-black/30 motion-reduce:transition-none dark:text-neutral-200 dark:hover:text-neutral-300 dark:focus:text-neutral-300 [&.active]:text-black/90 dark:[&.active]:text-neutral-400"
          href="#"
          id="dropdownMenuButton1"
          role="button"
          data-te-dropdown-toggle-ref
          aria-expanded="false">
          <!-- Dropdown trigger icon -->
          <span class="[&>svg]:w-5">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="currentColor"
              class="h-5 w-5">
              <path
                fill-rule="evenodd"
                d="M5.25 9a6.75 6.75 0 0113.5 0v.75c0 2.123.8 4.057 2.118 5.52a.75.75 0 01-.297 1.206c-1.544.57-3.16.99-4.831 1.243a3.75 3.75 0 11-7.48 0 24.585 24.585 0 01-4.831-1.244.75.75 0 01-.298-1.205A8.217 8.217 0 005.25 9.75V9zm4.502 8.9a2.25 2.25 0 104.496 0 25.057 25.057 0 01-4.496 0z"
                clip-rule="evenodd" />
            </svg>
          </span>
          <!-- Notification counter -->
          <span
            class="absolute -mt-4 ml-2.5 rounded-full bg-danger px-[0.35em] py-[0.15em] text-[0.6rem] font-bold leading-none text-white"
            >1</span
          >
        </a>
        <!-- First dropdown menu -->
        <ul
          class="absolute z-[1000] float-left m-0 hidden min-w-max list-none overflow-hidden rounded-lg border-none bg-white bg-clip-padding text-left text-base shadow-lg dark:bg-neutral-700 [&[data-te-dropdown-show]]:block"
          aria-labelledby="dropdownMenuButton1"
          data-te-dropdown-menu-ref>
          <!-- First dropdown menu items -->
          <li>
            <a
              class="block w-full whitespace-nowrap bg-transparent px-4 py-2 text-sm font-normal text-neutral-700 hover:bg-neutral-100 active:text-neutral-800 active:no-underline disabled:pointer-events-none disabled:bg-transparent disabled:text-neutral-400 dark:text-neutral-200 dark:hover:bg-white/30"
              href="#"
              data-te-dropdown-item-ref
              >Action</a
            >
          </li>
          <li>
            <a
              class="block w-full whitespace-nowrap bg-transparent px-4 py-2 text-sm font-normal text-neutral-700 hover:bg-neutral-100 active:text-neutral-800 active:no-underline disabled:pointer-events-none disabled:bg-transparent disabled:text-neutral-400 dark:text-neutral-200 dark:hover:bg-white/30"
              href="#"
              data-te-dropdown-item-ref
              >Another action</a
            >
          </li>
          <li>
            <a
              class="block w-full whitespace-nowrap bg-transparent px-4 py-2 text-sm font-normal text-neutral-700 hover:bg-neutral-100 active:text-neutral-800 active:no-underline disabled:pointer-events-none disabled:bg-transparent disabled:text-neutral-400 dark:text-neutral-200 dark:hover:bg-white/30"
              href="#"
              data-te-dropdown-item-ref
              >Something else here</a
            >
          </li>
        </ul>
      </div>

      <!-- Second dropdown container -->
      <div
        class="relative"
        data-te-dropdown-ref
        data-te-dropdown-alignment="end">
        <!-- Second dropdown trigger -->
        <a
          class="hidden-arrow flex items-center whitespace-nowrap transition duration-150 ease-in-out motion-reduce:transition-none"
          href="#"
          id="dropdownMenuButton2"
          role="button"
          data-te-dropdown-toggle-ref
          aria-expanded="false">
          <!-- User avatar -->
          <img
            src="https://tecdn.b-cdn.net/img/new/avatars/2.jpg"
            class="rounded-full"
            style="height: 25px; width: 25px"
            alt=""
            loading="lazy" />
        </a>
        <!-- Second dropdown menu -->
        <ul
          class="absolute z-[1000] float-left m-0 hidden min-w-max list-none overflow-hidden rounded-lg border-none bg-white bg-clip-padding text-left text-base shadow-lg dark:bg-neutral-700 [&[data-te-dropdown-show]]:block"
          aria-labelledby="dropdownMenuButton2"
          data-te-dropdown-menu-ref>
          <!-- Second dropdown menu items -->
          <li>
            <a
              class="block w-full whitespace-nowrap bg-transparent px-4 py-2 text-sm font-normal text-neutral-700 hover:bg-neutral-100 active:text-neutral-800 active:no-underline disabled:pointer-events-none disabled:bg-transparent disabled:text-neutral-400 dark:text-neutral-200 dark:hover:bg-white/30"
              href="#"
              data-te-dropdown-item-ref
              >Action</a
            >
          </li>
          <li>
            <a
              class="block w-full whitespace-nowrap bg-transparent px-4 py-2 text-sm font-normal text-neutral-700 hover:bg-neutral-100 active:text-neutral-800 active:no-underline disabled:pointer-events-none disabled:bg-transparent disabled:text-neutral-400 dark:text-neutral-200 dark:hover:bg-white/30"
              href="#"
              data-te-dropdown-item-ref
              >Another action</a
            >
          </li>
          <li>
            <a
              class="block w-full whitespace-nowrap bg-transparent px-4 py-2 text-sm font-normal text-neutral-700 hover:bg-neutral-100 active:text-neutral-800 active:no-underline disabled:pointer-events-none disabled:bg-transparent disabled:text-neutral-400 dark:text-neutral-200 dark:hover:bg-white/30"
              href="#"
              data-te-dropdown-item-ref
              >Something else here</a
            >
          </li>
        </ul>
      </div>
    </div>
  </div>
</nav>




   
   <!-- component -->
<div class="container mx-auto p-4">
      <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
        <div class="grid gap-4">
          <div>
            <!-- source https://tailwindcss.com/ -->
<div class="mt-6 sm:mt-10 relative z-10 rounded-xl shadow-xl">
    <div
        class="bg-white border-slate-100 transition-all duration-500 dark:bg-slate-800 transition-all duration-500 dark:border-slate-500 border-b rounded-t-xl p-4 pb-6 sm:p-10 sm:pb-8 lg:p-6 xl:p-10 xl:pb-8 space-y-6 sm:space-y-8 lg:space-y-6 xl:space-y-8">
        <div class="flex items-center space-x-4">
            <img src="https://tailwindcss.com/_next/static/media/full-stack-radio.afb14e4e.png" loading="lazy" decoding="async" alt="" class="flex-none rounded-lg bg-slate-100" width="88" height="88">
            <div class="min-w-0 flex-auto space-y-1 font-semibold">
                <p class="text-cyan-500 transition-all duration-500 dark:text-cyan-400 text-sm leading-6">
                    <abbr title="Episode">Ep.</abbr> 128
                </p>
                <h2 class="text-slate-500 transition-all duration-500 dark:text-slate-400 text-sm leading-6 truncate">
                    Scaling CSS at Heroku with Utility Classes
                </h2>
                <p class="text-slate-900 transition-all duration-500 dark:text-slate-50 text-lg">
                    Full Stack Radio
                </p>
            </div>
        </div>
        <div class="space-y-2">
            <div class="relative">
                <div class="bg-slate-100 transition-all duration-500 dark:bg-slate-700 rounded-full overflow-hidden">
                    <div class="bg-cyan-500 transition-all duration-500 dark:bg-cyan-400 w-1/2 h-2" role="progressbar"
                        aria-label="music progress" aria-valuenow="1456" aria-valuemin="0" aria-valuemax="4550"></div>
                </div>
                <div
                    class="ring-cyan-500 transition-all duration-500 dark:ring-cyan-400 ring-2 absolute left-1/2 top-1/2 w-4 h-4 -mt-2 -ml-2 flex items-center justify-center bg-white rounded-full shadow">
                    <div
                        class="w-1.5 h-1.5 bg-cyan-500 transition-all duration-500 dark:bg-cyan-400 rounded-full ring-1 ring-inset ring-slate-900/5">
                    </div>
                </div>
            </div>
            <div class="flex justify-between text-sm leading-6 font-medium tabular-nums">
                <div class="text-cyan-500 transition-all duration-500 dark:text-slate-100">24:16</div>
                <div class="text-slate-500 transition-all duration-500 dark:text-slate-400">75:50</div>
            </div>
        </div>
    </div>
    <div
        class="bg-slate-50 text-slate-500 transition-all duration-500 dark:bg-slate-600 transition-all duration-500 dark:text-slate-200 rounded-b-xl flex items-center">
        <div class="flex-auto flex items-center justify-evenly">
            <button type="button" aria-label="Add to favorites">
      <svg width="24" height="24">
        <path d="M7 6.931C7 5.865 7.853 5 8.905 5h6.19C16.147 5 17 5.865 17 6.931V19l-5-4-5 4V6.931Z" fill="currentColor" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
            <button type="button" class="hidden sm:block lg:hidden xl:block" aria-label="Previous">
      <svg width="24" height="24" fill="none">
        <path d="m10 12 8-6v12l-8-6Z" fill="currentColor" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
        <path d="M6 6v12" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
            <button type="button" aria-label="Rewind 10 seconds">
      <svg width="24" height="24" fill="none">
        <path d="M6.492 16.95c2.861 2.733 7.5 2.733 10.362 0 2.861-2.734 2.861-7.166 0-9.9-2.862-2.733-7.501-2.733-10.362 0A7.096 7.096 0 0 0 5.5 8.226" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
        <path d="M5 5v3.111c0 .491.398.889.889.889H9" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
        </div>
        <button type="button" class="bg-white text-slate-900 transition-all duration-500 dark:bg-slate-100 transition-all duration-500 dark:text-slate-700 flex-none -my-2 mx-auto w-20 h-20 rounded-full ring-1 ring-slate-900/5 shadow-md flex items-center justify-center" aria-label="Pause">
    <svg width="30" height="32" fill="currentColor">
      <rect x="6" y="4" width="4" height="24" rx="2"></rect>
      <rect x="20" y="4" width="4" height="24" rx="2"></rect>
    </svg>
  </button>
        <div class="flex-auto flex items-center justify-evenly">
            <button type="button" aria-label="Skip 10 seconds" class="">
      <svg width="24" height="24" fill="none">
        <path d="M17.509 16.95c-2.862 2.733-7.501 2.733-10.363 0-2.861-2.734-2.861-7.166 0-9.9 2.862-2.733 7.501-2.733 10.363 0 .38.365.711.759.991 1.176" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
        <path d="M19 5v3.111c0 .491-.398.889-.889.889H15" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
            <button type="button" class="hidden sm:block lg:hidden xl:block" aria-label="Next">
      <svg width="24" height="24" fill="none">
        <path d="M14 12 6 6v12l8-6Z" fill="currentColor" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
        <path d="M18 6v12" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
            <button type="button" class="rounded-lg text-xs leading-6 font-semibold px-2 ring-2 ring-inset ring-slate-500 text-slate-500 transition-all duration-500 dark:text-slate-100 transition-all duration-500 dark:ring-0 transition-all duration-500 dark:bg-slate-500">
      1x
    </button>
        </div>
    </div>
</div>
           
            
          </div>
          <div>
            <!-- source https://tailwindcss.com/ -->
<div class="mt-6 sm:mt-10 relative z-10 rounded-xl shadow-xl">
    <div
        class="bg-white border-slate-100 transition-all duration-500 dark:bg-slate-800 transition-all duration-500 dark:border-slate-500 border-b rounded-t-xl p-4 pb-6 sm:p-10 sm:pb-8 lg:p-6 xl:p-10 xl:pb-8 space-y-6 sm:space-y-8 lg:space-y-6 xl:space-y-8">
        <div class="flex items-center space-x-4">
            <img src="/img/Escudos/La Paz.gif" loading="lazy" decoding="async" alt="" class="flex-none rounded-lg bg-slate-100" width="88" height="88">

            <div class="min-w-0 flex-auto space-y-1 font-semibold">
                <p class="text-cyan-500 transition-all duration-500 dark:text-cyan-400 text-sm leading-6">
                    <abbr title="Episode">Ep.</abbr> 128
                </p>
                <h2 class="text-slate-500 transition-all duration-500 dark:text-slate-400 text-sm leading-6 truncate">
                    Scaling CSS at Heroku with Utility Classes
                </h2>
                <p class="text-slate-900 transition-all duration-500 dark:text-slate-50 text-lg">
                    Full Stack Radio
                </p>
            </div>
        </div>
        <div class="space-y-2">
            <div class="relative">
                <div class="bg-slate-100 transition-all duration-500 dark:bg-slate-700 rounded-full overflow-hidden">
                    <div class="bg-cyan-500 transition-all duration-500 dark:bg-cyan-400 w-1/2 h-2" role="progressbar"
                        aria-label="music progress" aria-valuenow="1456" aria-valuemin="0" aria-valuemax="4550"></div>
                </div>
                <div
                    class="ring-cyan-500 transition-all duration-500 dark:ring-cyan-400 ring-2 absolute left-1/2 top-1/2 w-4 h-4 -mt-2 -ml-2 flex items-center justify-center bg-white rounded-full shadow">
                    <div
                        class="w-1.5 h-1.5 bg-cyan-500 transition-all duration-500 dark:bg-cyan-400 rounded-full ring-1 ring-inset ring-slate-900/5">
                    </div>
                </div>
            </div>
            <div class="flex justify-between text-sm leading-6 font-medium tabular-nums">
                <div class="text-cyan-500 transition-all duration-500 dark:text-slate-100">24:16</div>
                <div class="text-slate-500 transition-all duration-500 dark:text-slate-400">75:50</div>
            </div>
        </div>
    </div>
    <div
        class="bg-slate-50 text-slate-500 transition-all duration-500 dark:bg-slate-600 transition-all duration-500 dark:text-slate-200 rounded-b-xl flex items-center">
        <div class="flex-auto flex items-center justify-evenly">
            <button type="button" aria-label="Add to favorites">
      <svg width="24" height="24">
        <path d="M7 6.931C7 5.865 7.853 5 8.905 5h6.19C16.147 5 17 5.865 17 6.931V19l-5-4-5 4V6.931Z" fill="currentColor" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
            <button type="button" class="hidden sm:block lg:hidden xl:block" aria-label="Previous">
      <svg width="24" height="24" fill="none">
        <path d="m10 12 8-6v12l-8-6Z" fill="currentColor" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
        <path d="M6 6v12" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
            <button type="button" aria-label="Rewind 10 seconds">
      <svg width="24" height="24" fill="none">
        <path d="M6.492 16.95c2.861 2.733 7.5 2.733 10.362 0 2.861-2.734 2.861-7.166 0-9.9-2.862-2.733-7.501-2.733-10.362 0A7.096 7.096 0 0 0 5.5 8.226" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
        <path d="M5 5v3.111c0 .491.398.889.889.889H9" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
        </div>
        <button type="button" class="bg-white text-slate-900 transition-all duration-500 dark:bg-slate-100 transition-all duration-500 dark:text-slate-700 flex-none -my-2 mx-auto w-20 h-20 rounded-full ring-1 ring-slate-900/5 shadow-md flex items-center justify-center" aria-label="Pause">
    <svg width="30" height="32" fill="currentColor">
      <rect x="6" y="4" width="4" height="24" rx="2"></rect>
      <rect x="20" y="4" width="4" height="24" rx="2"></rect>
    </svg>
  </button>
        <div class="flex-auto flex items-center justify-evenly">
            <button type="button" aria-label="Skip 10 seconds" class="">
      <svg width="24" height="24" fill="none">
        <path d="M17.509 16.95c-2.862 2.733-7.501 2.733-10.363 0-2.861-2.734-2.861-7.166 0-9.9 2.862-2.733 7.501-2.733 10.363 0 .38.365.711.759.991 1.176" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
        <path d="M19 5v3.111c0 .491-.398.889-.889.889H15" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
            <button type="button" class="hidden sm:block lg:hidden xl:block" aria-label="Next">
      <svg width="24" height="24" fill="none">
        <path d="M14 12 6 6v12l8-6Z" fill="currentColor" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
        <path d="M18 6v12" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
            <button type="button" class="rounded-lg text-xs leading-6 font-semibold px-2 ring-2 ring-inset ring-slate-500 text-slate-500 transition-all duration-500 dark:text-slate-100 transition-all duration-500 dark:ring-0 transition-all duration-500 dark:bg-slate-500">
      1x
    </button>
        </div>
    </div>
</div>
      
          </div>
          <div>

            <!-- source https://tailwindcss.com/ -->
<div class="mt-6 sm:mt-10 relative z-10 rounded-xl shadow-xl">
    <div
        class="bg-white border-slate-100 transition-all duration-500 dark:bg-slate-800 transition-all duration-500 dark:border-slate-500 border-b rounded-t-xl p-4 pb-6 sm:p-10 sm:pb-8 lg:p-6 xl:p-10 xl:pb-8 space-y-6 sm:space-y-8 lg:space-y-6 xl:space-y-8">
        <div class="flex items-center space-x-4">
            <img src="https://tailwindcss.com/_next/static/media/full-stack-radio.afb14e4e.png" loading="lazy" decoding="async" alt="" class="flex-none rounded-lg bg-slate-100" width="88" height="88">
            <div class="min-w-0 flex-auto space-y-1 font-semibold">
                <p class="text-cyan-500 transition-all duration-500 dark:text-cyan-400 text-sm leading-6">
                    <abbr title="Episode">Ep.</abbr> 128
                </p>
                <h2 class="text-slate-500 transition-all duration-500 dark:text-slate-400 text-sm leading-6 truncate">
                    Scaling CSS at Heroku with Utility Classes
                </h2>
                <p class="text-slate-900 transition-all duration-500 dark:text-slate-50 text-lg">
                    Full Stack Radio
                </p>
            </div>
        </div>
        <div class="space-y-2">
            <div class="relative">
                <div class="bg-slate-100 transition-all duration-500 dark:bg-slate-700 rounded-full overflow-hidden">
                    <div class="bg-cyan-500 transition-all duration-500 dark:bg-cyan-400 w-1/2 h-2" role="progressbar"
                        aria-label="music progress" aria-valuenow="1456" aria-valuemin="0" aria-valuemax="4550"></div>
                </div>
                <div
                    class="ring-cyan-500 transition-all duration-500 dark:ring-cyan-400 ring-2 absolute left-1/2 top-1/2 w-4 h-4 -mt-2 -ml-2 flex items-center justify-center bg-white rounded-full shadow">
                    <div
                        class="w-1.5 h-1.5 bg-cyan-500 transition-all duration-500 dark:bg-cyan-400 rounded-full ring-1 ring-inset ring-slate-900/5">
                    </div>
                </div>
            </div>
            <div class="flex justify-between text-sm leading-6 font-medium tabular-nums">
                <div class="text-cyan-500 transition-all duration-500 dark:text-slate-100">24:16</div>
                <div class="text-slate-500 transition-all duration-500 dark:text-slate-400">75:50</div>
            </div>
        </div>
    </div>
    <div
        class="bg-slate-50 text-slate-500 transition-all duration-500 dark:bg-slate-600 transition-all duration-500 dark:text-slate-200 rounded-b-xl flex items-center">
        <div class="flex-auto flex items-center justify-evenly">
            <button type="button" aria-label="Add to favorites">
      <svg width="24" height="24">
        <path d="M7 6.931C7 5.865 7.853 5 8.905 5h6.19C16.147 5 17 5.865 17 6.931V19l-5-4-5 4V6.931Z" fill="currentColor" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
            <button type="button" class="hidden sm:block lg:hidden xl:block" aria-label="Previous">
      <svg width="24" height="24" fill="none">
        <path d="m10 12 8-6v12l-8-6Z" fill="currentColor" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
        <path d="M6 6v12" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
            <button type="button" aria-label="Rewind 10 seconds">
      <svg width="24" height="24" fill="none">
        <path d="M6.492 16.95c2.861 2.733 7.5 2.733 10.362 0 2.861-2.734 2.861-7.166 0-9.9-2.862-2.733-7.501-2.733-10.362 0A7.096 7.096 0 0 0 5.5 8.226" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
        <path d="M5 5v3.111c0 .491.398.889.889.889H9" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
        </div>
        <button type="button" class="bg-white text-slate-900 transition-all duration-500 dark:bg-slate-100 transition-all duration-500 dark:text-slate-700 flex-none -my-2 mx-auto w-20 h-20 rounded-full ring-1 ring-slate-900/5 shadow-md flex items-center justify-center" aria-label="Pause">
    <svg width="30" height="32" fill="currentColor">
      <rect x="6" y="4" width="4" height="24" rx="2"></rect>
      <rect x="20" y="4" width="4" height="24" rx="2"></rect>
    </svg>
  </button>
        <div class="flex-auto flex items-center justify-evenly">
            <button type="button" aria-label="Skip 10 seconds" class="">
      <svg width="24" height="24" fill="none">
        <path d="M17.509 16.95c-2.862 2.733-7.501 2.733-10.363 0-2.861-2.734-2.861-7.166 0-9.9 2.862-2.733 7.501-2.733 10.363 0 .38.365.711.759.991 1.176" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
        <path d="M19 5v3.111c0 .491-.398.889-.889.889H15" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
            <button type="button" class="hidden sm:block lg:hidden xl:block" aria-label="Next">
      <svg width="24" height="24" fill="none">
        <path d="M14 12 6 6v12l8-6Z" fill="currentColor" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
        <path d="M18 6v12" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </button>
            <button type="button" class="rounded-lg text-xs leading-6 font-semibold px-2 ring-2 ring-inset ring-slate-500 text-slate-500 transition-all duration-500 dark:text-slate-100 transition-all duration-500 dark:ring-0 transition-all duration-500 dark:bg-slate-500">
      1x
    </button>
        </div>
    </div>
</div>
            <img
              class="h-auto max-w-full rounded-lg"
              src="/img/Escudos/La Paz.gif"
              alt=""
            />
          </div>
        </div>
        <div class="grid gap-4">
          <div>
            <img
              class="h-auto max-w-full rounded-lg"
              src="/img/Escudos/Litoral.gif"
              alt=""
            />
          </div>
          <div>
            <img
              class="h-auto max-w-full rounded-lg"
              src="/img/Escudos/Oruro.gif"
              alt=""
            />
          </div>
          <div>
            <img
              class="h-auto max-w-full rounded-lg"
              src="/img/Escudos/Pando.gif"
              alt=""
            />
          </div>
        </div>
        <div class="grid gap-4">
          <div>
            <img
              class="h-auto max-w-full rounded-lg"
              src="/img/Escudos/Potosi.gif"
              alt=""
            />
          </div>
          <div>
            <img
              class="h-auto max-w-full rounded-lg"
              src="/img/Escudos/Santa Cruz.gif"
              alt=""
            />
          </div>
          <div>
            <img
              class="h-auto max-w-full rounded-lg"
              src="/img/Escudos/Sucre.gif"
              alt=""
            />
          </div>
        </div>
        <div class="grid gap-4">
          <div>
            <img
              class="h-auto max-w-full rounded-lg"
              src="/img/Escudos/Tarija.gif"
              alt=""
            />
          </div>
        </div>
      </div>
    </div>

<!--Footer container-->
<footer
  class="flex flex-col items-center bg-neutral-200 text-center text-white dark:bg-black">
  <div class="container pt-9">
    <div class="mb-9 flex justify-center">
      <a href="#!" class="mr-9 text-neutral-800 dark:text-neutral-200">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-4 w-4"
          fill="currentColor"
          viewBox="0 0 24 24">
          <path
            d="M9 8h-3v4h3v12h5v-12h3.642l.358-4h-4v-1.667c0-.955.192-1.333 1.115-1.333h2.885v-5h-3.808c-3.596 0-5.192 1.583-5.192 4.615v3.385z" />
        </svg>
      </a>
      <a href="#!" class="mr-9 text-neutral-800 dark:text-neutral-200">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-4 w-4"
          fill="currentColor"
          viewBox="0 0 24 24">
          <path
            d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z" />
        </svg>
      </a>
      <a href="#!" class="mr-9 text-neutral-800 dark:text-neutral-200">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-5 w-5"
          fill="currentColor"
          viewBox="0 0 24 24">
          <path
            d="M7 11v2.4h3.97c-.16 1.029-1.2 3.02-3.97 3.02-2.39 0-4.34-1.979-4.34-4.42 0-2.44 1.95-4.42 4.34-4.42 1.36 0 2.27.58 2.79 1.08l1.9-1.83c-1.22-1.14-2.8-1.83-4.69-1.83-3.87 0-7 3.13-7 7s3.13 7 7 7c4.04 0 6.721-2.84 6.721-6.84 0-.46-.051-.81-.111-1.16h-6.61zm0 0 17 2h-3v3h-2v-3h-3v-2h3v-3h2v3h3v2z"
            fill-rule="evenodd"
            clip-rule="evenodd" />
        </svg>
      </a>
      <a href="#!" class="mr-9 text-neutral-800 dark:text-neutral-200">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-4 w-4"
          fill="currentColor"
          viewBox="0 0 24 24">
          <path
            d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z" />
        </svg>
      </a>
      <a href="#!" class="mr-9 text-neutral-800 dark:text-neutral-200">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-4 w-4"
          fill="currentColor"
          viewBox="0 0 24 24">
          <path
            d="M4.98 3.5c0 1.381-1.11 2.5-2.48 2.5s-2.48-1.119-2.48-2.5c0-1.38 1.11-2.5 2.48-2.5s2.48 1.12 2.48 2.5zm.02 4.5h-5v16h5v-16zm7.982 0h-4.968v16h4.969v-8.399c0-4.67 6.029-5.052 6.029 0v8.399h4.988v-10.131c0-7.88-8.922-7.593-11.018-3.714v-2.155z" />
        </svg>
      </a>
      <a href="#!" class="text-neutral-800 dark:text-neutral-200">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-4 w-4"
          fill="currentColor"
          viewBox="0 0 24 24">
          <path
            d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z" />
        </svg>
      </a>
    </div>
  </div>

  <!--Copyright section-->
  <div
    class="w-full bg-neutral-300 p-4 text-center text-neutral-700 dark:bg-black dark:text-neutral-200">
    © 2023 Copyright
    <a
      class="text-neutral-800 dark:text-neutral-400"
      href="https://yovanenovore.tech"
      >Yovan Enovore</a
    >
  </div>
</footer>

</template>

<style>
.bg-dots-darker {
    background-image: url("data:image/svg+xml,%3Csvg width='30' height='30' viewBox='0 0 30 30' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1.22676 0C1.91374 0 2.45351 0.539773 2.45351 1.22676C2.45351 1.91374 1.91374 2.45351 1.22676 2.45351C0.539773 2.45351 0 1.91374 0 1.22676C0 0.539773 0.539773 0 1.22676 0Z' fill='rgba(0,0,0,0.07)'/%3E%3C/svg%3E");
}
@media (prefers-color-scheme: dark) {
    .dark\:bg-dots-lighter {
        background-image: url("data:image/svg+xml,%3Csvg width='30' height='30' viewBox='0 0 30 30' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1.22676 0C1.91374 0 2.45351 0.539773 2.45351 1.22676C2.45351 1.91374 1.91374 2.45351 1.22676 2.45351C0.539773 2.45351 0 1.91374 0 1.22676C0 0.539773 0.539773 0 1.22676 0Z' fill='rgba(255,255,255,0.07)'/%3E%3C/svg%3E");
                    }
}
</style>
