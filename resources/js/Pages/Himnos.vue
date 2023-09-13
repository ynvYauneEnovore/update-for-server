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
        type="button" data-te-collapse-init data-te-target="#navbarSupportedContent1"
        aria-controls="navbarSupportedContent1" aria-expanded="false" aria-label="Toggle navigation">
        <!-- Hamburger icon -->
        <span class="[&>svg]:w-7">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="h-7 w-7">
            <path fill-rule="evenodd"
              d="M3 6.75A.75.75 0 013.75 6h16.5a.75.75 0 010 1.5H3.75A.75.75 0 013 6.75zM3 12a.75.75 0 01.75-.75h16.5a.75.75 0 010 1.5H3.75A.75.75 0 013 12zm0 5.25a.75.75 0 01.75-.75h16.5a.75.75 0 010 1.5H3.75a.75.75 0 01-.75-.75z"
              clip-rule="evenodd" />
          </svg>
        </span>
      </button>

      <!-- Collapsible navigation container -->
      <div class="!visible hidden flex-grow basis-[100%] items-center lg:!flex lg:basis-auto" id="navbarSupportedContent1"
        data-te-collapse-item>
        <!-- Logo -->
        <a class="mb-6 ml-2 mr-5 mt-3 flex items-center text-neutral-900 hover:text-neutral-900 focus:text-neutral-900 dark:text-neutral-200 dark:hover:text-neutral-400 dark:focus:text-neutral-400 lg:mb-0 lg:mt-0"
          href="https://yovanenovore.tech">
          <img src="https://raw.githubusercontent.com/ynvYauneEnovore/personal-port/main/public/img/ynv.png"
            style="height: 50px" alt="TE Logo" loading="lazy" />
        </a>
        <!-- Left navigation links -->
        <ul class="list-style-none mr-auto flex flex-col pl-0 lg:flex-row" data-te-navbar-nav-ref>
          <li class="mb-4 lg:mb-0 lg:pr-2" data-te-nav-item-ref>
            <!-- Dashboard link -->
            <a class="text-neutral-500 transition duration-200 hover:text-neutral-700 hover:ease-in-out focus:text-neutral-700 disabled:text-black/30 motion-reduce:transition-none dark:text-neutral-200 dark:hover:text-neutral-300 dark:focus:text-neutral-300 lg:px-2 [&.active]:text-black/90 dark:[&.active]:text-zinc-400 active"
              href="#" data-te-nav-link-ref>Himnos</a>
          </li>
          <!-- Team link -->
          <li class="mb-4 lg:mb-0 lg:pr-2" data-te-nav-item-ref>
            <a class="text-neutral-500 transition duration-200 hover:text-neutral-700 hover:ease-in-out focus:text-neutral-700 disabled:text-black/30 motion-reduce:transition-none dark:text-neutral-200 dark:hover:text-neutral-300 dark:focus:text-neutral-300 lg:px-2 [&.active]:text-black/90 dark:[&.active]:text-neutral-400"
              href="#" data-te-nav-link-ref>Mapas</a>
          </li>
          <!-- Projects link -->
          <li class="mb-4 lg:mb-0 lg:pr-2" data-te-nav-item-ref>
            <a class="text-neutral-500 transition duration-200 hover:text-neutral-700 hover:ease-in-out focus:text-neutral-700 disabled:text-black/30 motion-reduce:transition-none dark:text-neutral-200 dark:hover:text-neutral-300 dark:focus:text-neutral-300 lg:px-2 [&.active]:text-black/90 dark:[&.active]:text-neutral-400"
              href="#" data-te-nav-link-ref>Simbolos</a>
          </li>
        </ul>
      </div>

      <!-- Right elements -->
      <div class="relative flex items-center">

        <!-- Second dropdown container -->
        <div class="relative" data-te-dropdown-ref data-te-dropdown-alignment="end">
          <!-- Second dropdown trigger -->
          <a class="hidden-arrow flex items-center whitespace-nowrap transition duration-150 ease-in-out motion-reduce:transition-none"
            href="#" id="dropdownMenuButton2" role="button" data-te-dropdown-toggle-ref aria-expanded="false">
            <!-- User avatar -->
            <img src="https://www.svgrepo.com/show/405427/flag-for-flag-bolivia.svg" class=""
              style="height: 50px;" alt="" loading="lazy" />
          </a>
          <!-- Second dropdown menu -->
          <ul
            class="absolute z-[1000] float-left m-0 hidden min-w-max list-none overflow-hidden rounded-lg border-none bg-white bg-clip-padding text-left text-base shadow-lg dark:bg-neutral-700 [&[data-te-dropdown-show]]:block"
            aria-labelledby="dropdownMenuButton2" data-te-dropdown-menu-ref>
            <!-- Second dropdown menu items -->
            <li>
              <a class="block w-full whitespace-nowrap bg-transparent px-4 py-2 text-sm font-normal text-neutral-700 hover:bg-neutral-100 active:text-neutral-800 active:no-underline disabled:pointer-events-none disabled:bg-transparent disabled:text-neutral-400 dark:text-neutral-200 dark:hover:bg-white/30"
                href="#" data-te-dropdown-item-ref>Action</a>
            </li>
            <li>
              <a class="block w-full whitespace-nowrap bg-transparent px-4 py-2 text-sm font-normal text-neutral-700 hover:bg-neutral-100 active:text-neutral-800 active:no-underline disabled:pointer-events-none disabled:bg-transparent disabled:text-neutral-400 dark:text-neutral-200 dark:hover:bg-white/30"
                href="#" data-te-dropdown-item-ref>Another action</a>
            </li>
            <li>
              <a class="block w-full whitespace-nowrap bg-transparent px-4 py-2 text-sm font-normal text-neutral-700 hover:bg-neutral-100 active:text-neutral-800 active:no-underline disabled:pointer-events-none disabled:bg-transparent disabled:text-neutral-400 dark:text-neutral-200 dark:hover:bg-white/30"
                href="#" data-te-dropdown-item-ref>Something else here</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </nav>



<article x-data="slider" class="relative w-full flex flex-shrink-0 overflow-hidden shadow-2xl">
    <div class="rounded-full bg-gray-600 text-white absolute top-5 right-5 text-sm px-2 text-center z-10">
        <span x-text="currentIndex"></span>/
        <span x-text="images.length"></span>
    </div>

    <template x-for="(image, index) in images">
        <figure class="h-96" x-show="currentIndex == index + 1" x-transition:enter="transition transform duration-300"
        x-transition:enter-start="opacity-0" x-transition:enter-end="opacity-100"
        x-transition:leave="transition transform duration-300" x-transition:leave-start="opacity-100"
        x-transition:leave-end="opacity-0">
        <img :src="image" alt="Image" class="absolute inset-0 z-10 h-full w-full object-cover opacity-70" />
        <figcaption class="absolute inset-x-0 bottom-1 z-20 w-96 mx-auto p-4 font-light text-sm text-center tracking-widest leading-snug bg-gray-300 bg-opacity-25">
            Any kind of content here!
            Primum in nostrane potestate est, quid meminerimus? Nulla erit controversia. Vestri haec verecundius, illi fortasse constantius. 
        </figcaption>
        </figure>
    </template>

    <button @click="back()"
        class="absolute left-14 top-1/2 -translate-y-1/2 w-11 h-11 flex justify-center items-center rounded-full shadow-md z-10 bg-gray-100 hover:bg-gray-200">
        <svg class=" w-8 h-8 font-bold transition duration-500 ease-in-out transform motion-reduce:transform-none text-gray-500 hover:text-gray-600 hover:-translate-x-0.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M15 19l-7-7 7-7">
            </path>
        </svg>
    </button>

    <button @click="next()"
    class="absolute right-14 top-1/2 translate-y-1/2 w-11 h-11 flex justify-center items-center rounded-full shadow-md z-10 bg-gray-100 hover:bg-gray-200">
        <svg class=" w-8 h-8 font-bold transition duration-500 ease-in-out transform motion-reduce:transform-none text-gray-500 hover:text-gray-600 hover:translate-x-0.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"
        xmlns="http://www.w3.org/2000/svg">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M9 5l7 7-7 7"></path>
        </svg>
    </button>
</article>




  <!-- component -->
  <div class="container mx-auto p-4">
    <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
      <div class="grid gap-4">
        <div>
          <!-- reproductor -->
          <div class="mt-1 sm:mt-1 relative z-10 rounded-xl shadow-xl">
            <div
              class="bg-white border-slate-100 transition-all duration-500 dark:bg-slate-800 transition-all duration-500 dark:border-slate-500 border-b rounded-t-xl p-4 pb-6 sm:p-10 sm:pb-8 lg:p-6 xl:p-10 xl:pb-8 space-y-6 sm:space-y-8 lg:space-y-6 xl:space-y-8">
              <div class="flex items-center space-x-4">
                <img src="/img/Escudos/Beni.gif" loading="lazy" decoding="async" alt=""
                  class="flex-none rounded-lg bg-slate-100" width="88" height="88">
                <div class="min-w-0 flex-auto space-y-1 font-semibold">
                  <p class="text-cyan-500 transition-all duration-500 dark:text-cyan-400 text-sm leading-6">
                    <abbr title="Episode">Dpto.</abbr> Beni
                  </p>
                  <h2 class="text-slate-500 transition-all duration-500 dark:text-slate-400 text-sm leading-6 truncate">
                    213.564 km²
                  </h2>
                  <p class="text-slate-900 transition-all duration-500 dark:text-slate-50 text-lg">
                    18-11-1842
                  </p>
                </div>
              </div>
            </div>
            <div
              class="bg-slate-50 text-slate-500 transition-all duration-500 dark:bg-slate-600 transition-all duration-500 dark:text-slate-200 rounded-b-xl flex items-center">
              <div class="flex-auto flex items-center justify-evenly">
                <audio controls>
                  <source src="Himnos/Beni.mp3" type="audio/mpeg">
                  Tu navegador no admite la reproducción de audio.
                </audio>
              </div>
            </div>
          </div>
          <!-- fin reproductor -->

          <!-- reproductor -->
          <div class="mt-1 sm:mt-5 relative z-10 rounded-xl shadow-xl">
            <div
              class="bg-white border-slate-100 transition-all duration-500 dark:bg-slate-800 transition-all duration-500 dark:border-slate-500 border-b rounded-t-xl p-4 pb-6 sm:p-10 sm:pb-8 lg:p-6 xl:p-10 xl:pb-8 space-y-6 sm:space-y-8 lg:space-y-6 xl:space-y-8">
              <div class="flex items-center space-x-4">
                <img src="/img/Escudos/La Paz.gif" loading="lazy" decoding="async" alt=""
                  class="flex-none rounded-lg bg-slate-100" width="88" height="88">
                <div class="min-w-0 flex-auto space-y-1 font-semibold">
                  <p class="text-cyan-500 transition-all duration-500 dark:text-cyan-400 text-sm leading-6">
                    <abbr title="Episode">Dpto.</abbr> La Paz
                  </p>
                  <h2 class="text-slate-500 transition-all duration-500 dark:text-slate-400 text-sm leading-6 truncate">
                    213.564 km²
                  </h2>
                  <p class="text-slate-900 transition-all duration-500 dark:text-slate-50 text-lg">
                    18-11-1842
                  </p>
                </div>
              </div>
            </div>
            <div
              class="bg-slate-50 text-slate-500 transition-all duration-500 dark:bg-slate-600 transition-all duration-500 dark:text-slate-200 rounded-b-xl flex items-center">
              <div class="flex-auto flex items-center justify-evenly">
                <audio controls>
                  <source src="Himnos/La Paz.mp3" type="audio/mpeg">
                  Tu navegador no admite la reproducción de audio.
                </audio>
              </div>
            </div>
          </div>
          <!-- fin reproductor -->
     <!-- reproductor -->
     <div class="mt-1 sm:mt-5 relative z-10 rounded-xl shadow-xl">
            <div
              class="bg-white border-slate-100 transition-all duration-500 dark:bg-slate-800 transition-all duration-500 dark:border-slate-500 border-b rounded-t-xl p-4 pb-6 sm:p-10 sm:pb-8 lg:p-6 xl:p-10 xl:pb-8 space-y-6 sm:space-y-8 lg:space-y-6 xl:space-y-8">
              <div class="flex items-center space-x-4">
                <img src="/img/Escudos/Sucre.gif" loading="lazy" decoding="async" alt=""
                  class="flex-none rounded-lg bg-slate-100" width="88" height="88">
                <div class="min-w-0 flex-auto space-y-1 font-semibold">
                  <p class="text-cyan-500 transition-all duration-500 dark:text-cyan-400 text-sm leading-6">
                    <abbr title="Episode">Dpto.</abbr> Chuquisaca
                  </p>
                  <h2 class="text-slate-500 transition-all duration-500 dark:text-slate-400 text-sm leading-6 truncate">
                    213.564 km²
                  </h2>
                  <p class="text-slate-900 transition-all duration-500 dark:text-slate-50 text-lg">
                    18-11-1842
                  </p>
                </div>
              </div>
            </div>
            <div
              class="bg-slate-50 text-slate-500 transition-all duration-500 dark:bg-slate-600 transition-all duration-500 dark:text-slate-200 rounded-b-xl flex items-center">
              <div class="flex-auto flex items-center justify-evenly">
                <audio controls>
                  <source src="Himnos/Chuquisaca.mp3" type="audio/mpeg">
                  Tu navegador no admite la reproducción de audio.
                </audio>
              </div>
            </div>
          </div>
          <!-- fin reproductor -->

        </div>
      </div>

      <!-- reproductor -->
      <div>
        <div class="mt-1 sm:mt-1 relative z-10 rounded-xl shadow-xl">
          <div
            class="bg-white border-slate-100 transition-all duration-500 dark:bg-slate-800 transition-all duration-500 dark:border-slate-500 border-b rounded-t-xl p-4 pb-6 sm:p-10 sm:pb-8 lg:p-6 xl:p-10 xl:pb-8 space-y-6 sm:space-y-8 lg:space-y-6 xl:space-y-8">
            <div class="flex items-center space-x-4">
              <img src="/img/Escudos/Cochabamba.gif" loading="lazy" decoding="async" alt=""
                class="flex-none rounded-lg bg-slate-100" width="88" height="88">
              <div class="min-w-0 flex-auto space-y-1 font-semibold">
                <p class="text-cyan-500 transition-all duration-500 dark:text-cyan-400 text-sm leading-6">
                  <abbr title="Episode">Dpto.</abbr> Beni
                </p>
                <h2 class="text-slate-500 transition-all duration-500 dark:text-slate-400 text-sm leading-6 truncate">
                  213.564 km²
                </h2>
                <p class="text-slate-900 transition-all duration-500 dark:text-slate-50 text-lg">
                  18-11-1842
                </p>
              </div>
            </div>
          </div>
          <div
            class="bg-slate-50 text-slate-500 transition-all duration-500 dark:bg-slate-600 transition-all duration-500 dark:text-slate-200 rounded-b-xl flex items-center">
            <div class="flex-auto flex items-center justify-evenly">
              <audio controls>
                <source src="Himnos/Beni.mp3" type="audio/mpeg">
                Tu navegador no admite la reproducción de audio.
              </audio>
            </div>
          </div>
        </div>
        <!-- fin reproductor -->

        <!-- reproductor -->
        <div class="mt-1 sm:mt-5 relative z-10 rounded-xl shadow-xl">
          <div
            class="bg-white border-slate-100 transition-all duration-500 dark:bg-slate-800 transition-all duration-500 dark:border-slate-500 border-b rounded-t-xl p-4 pb-6 sm:p-10 sm:pb-8 lg:p-6 xl:p-10 xl:pb-8 space-y-6 sm:space-y-8 lg:space-y-6 xl:space-y-8">
            <div class="flex items-center space-x-4">
              <img src="/img/Escudos/Oruro.gif" loading="lazy" decoding="async" alt=""
                class="flex-none rounded-lg bg-slate-100" width="88" height="88">
              <div class="min-w-0 flex-auto space-y-1 font-semibold">
                <p class="text-cyan-500 transition-all duration-500 dark:text-cyan-400 text-sm leading-6">
                  <abbr title="Episode">Dpto.</abbr> Beni
                </p>
                <h2 class="text-slate-500 transition-all duration-500 dark:text-slate-400 text-sm leading-6 truncate">
                  213.564 km²
                </h2>
                <p class="text-slate-900 transition-all duration-500 dark:text-slate-50 text-lg">
                  18-11-1842
                </p>
              </div>
            </div>
          </div>
          <div
            class="bg-slate-50 text-slate-500 transition-all duration-500 dark:bg-slate-600 transition-all duration-500 dark:text-slate-200 rounded-b-xl flex items-center">
            <div class="flex-auto flex items-center justify-evenly">
              <audio controls>
                <source src="Himnos/Beni.mp3" type="audio/mpeg">
                Tu navegador no admite la reproducción de audio.
              </audio>
            </div>
          </div>
        </div>
        <!-- fin reproductor -->

             <!-- reproductor -->
             <div class="mt-1 sm:mt-5 relative z-10 rounded-xl shadow-xl">
            <div
              class="bg-white border-slate-100 transition-all duration-500 dark:bg-slate-800 transition-all duration-500 dark:border-slate-500 border-b rounded-t-xl p-4 pb-6 sm:p-10 sm:pb-8 lg:p-6 xl:p-10 xl:pb-8 space-y-6 sm:space-y-8 lg:space-y-6 xl:space-y-8">
              <div class="flex items-center space-x-4">
                <img src="/img/Escudos/Pando.gif" loading="lazy" decoding="async" alt=""
                  class="flex-none rounded-lg bg-slate-100" width="88" height="88">
                <div class="min-w-0 flex-auto space-y-1 font-semibold">
                  <p class="text-cyan-500 transition-all duration-500 dark:text-cyan-400 text-sm leading-6">
                    <abbr title="Episode">Dpto.</abbr> Beni
                  </p>
                  <h2 class="text-slate-500 transition-all duration-500 dark:text-slate-400 text-sm leading-6 truncate">
                    213.564 km²
                  </h2>
                  <p class="text-slate-900 transition-all duration-500 dark:text-slate-50 text-lg">
                    18-11-1842
                  </p>
                </div>
              </div>
            </div>
            <div
              class="bg-slate-50 text-slate-500 transition-all duration-500 dark:bg-slate-600 transition-all duration-500 dark:text-slate-200 rounded-b-xl flex items-center">
              <div class="flex-auto flex items-center justify-evenly">
                <audio controls>
                  <source src="Himnos/Beni.mp3" type="audio/mpeg">
                  Tu navegador no admite la reproducción de audio.
                </audio>
              </div>
            </div>
          </div>
          <!-- fin reproductor -->
      </div>
      <div>
        <!-- reproductor -->
        <div class="mt-1 sm:mt-1 relative z-10 rounded-xl shadow-xl">
          <div
            class="bg-white border-slate-100 transition-all duration-500 dark:bg-slate-800 transition-all duration-500 dark:border-slate-500 border-b rounded-t-xl p-4 pb-6 sm:p-10 sm:pb-8 lg:p-6 xl:p-10 xl:pb-8 space-y-6 sm:space-y-8 lg:space-y-6 xl:space-y-8">
            <div class="flex items-center space-x-4">
              <img src="/img/Escudos/Potosi.gif" loading="lazy" decoding="async" alt=""
                class="flex-none rounded-lg bg-slate-100" width="88" height="88">
              <div class="min-w-0 flex-auto space-y-1 font-semibold">
                <p class="text-cyan-500 transition-all duration-500 dark:text-cyan-400 text-sm leading-6">
                  <abbr title="Episode">Dpto.</abbr> Beni
                </p>
                <h2 class="text-slate-500 transition-all duration-500 dark:text-slate-400 text-sm leading-6 truncate">
                  213.564 km²
                </h2>
                <p class="text-slate-900 transition-all duration-500 dark:text-slate-50 text-lg">
                  18-11-1842
                </p>
              </div>
            </div>
          </div>
          <div
            class="bg-slate-50 text-slate-500 transition-all duration-500 dark:bg-slate-600 transition-all duration-500 dark:text-slate-200 rounded-b-xl flex items-center">
            <div class="flex-auto flex items-center justify-evenly">
              <audio controls>
                <source src="Himnos/Beni.mp3" type="audio/mpeg">
                Tu navegador no admite la reproducción de audio.
              </audio>
            </div>
          </div>
        </div>
        <!-- fin reproductor -->

        <!-- reproductor -->
        <div class="mt-1 sm:mt-5 relative z-10 rounded-xl shadow-xl">
          <div
            class="bg-white border-slate-100 transition-all duration-500 dark:bg-slate-800 transition-all duration-500 dark:border-slate-500 border-b rounded-t-xl p-4 pb-6 sm:p-10 sm:pb-8 lg:p-6 xl:p-10 xl:pb-8 space-y-6 sm:space-y-8 lg:space-y-6 xl:space-y-8">
            <div class="flex items-center space-x-4">
              <img src="/img/Escudos/Santa Cruz.gif" loading="lazy" decoding="async" alt=""
                class="flex-none rounded-lg bg-slate-100" width="88" height="88">
              <div class="min-w-0 flex-auto space-y-1 font-semibold">
                <p class="text-cyan-500 transition-all duration-500 dark:text-cyan-400 text-sm leading-6">
                  <abbr title="Episode">Dpto.</abbr> Beni
                </p>
                <h2 class="text-slate-500 transition-all duration-500 dark:text-slate-400 text-sm leading-6 truncate">
                  213.564 km²
                </h2>
                <p class="text-slate-900 transition-all duration-500 dark:text-slate-50 text-lg">
                  18-11-1842
                </p>
              </div>
            </div>
          </div>
          <div
            class="bg-slate-50 text-slate-500 transition-all duration-500 dark:bg-slate-600 transition-all duration-500 dark:text-slate-200 rounded-b-xl flex items-center">
            <div class="flex-auto flex items-center justify-evenly">
              <audio controls>
                <source src="Himnos/Beni.mp3" type="audio/mpeg">
                Tu navegador no admite la reproducción de audio.
              </audio>
            </div>
          </div>
        </div>
        <!-- fin reproductor -->
      </div>


      <div>
        <!-- reproductor -->
        <div class="mt-1 sm:mt-1 relative z-10 rounded-xl shadow-xl">
          <div
            class="bg-white border-slate-100 transition-all duration-500 dark:bg-slate-800 transition-all duration-500 dark:border-slate-500 border-b rounded-t-xl p-4 pb-6 sm:p-10 sm:pb-8 lg:p-6 xl:p-10 xl:pb-8 space-y-6 sm:space-y-8 lg:space-y-6 xl:space-y-8">
            <div class="flex items-center space-x-4">
              <img src="/img/Escudos/Tarija.gif" loading="lazy" decoding="async" alt=""
                class="flex-none rounded-lg bg-slate-100" width="88" height="88">
              <div class="min-w-0 flex-auto space-y-1 font-semibold">
                <p class="text-cyan-500 transition-all duration-500 dark:text-cyan-400 text-sm leading-6">
                  <abbr title="Episode">Dpto.</abbr> Beni
                </p>
                <h2 class="text-slate-500 transition-all duration-500 dark:text-slate-400 text-sm leading-6 truncate">
                  213.564 km²
                </h2>
                <p class="text-slate-900 transition-all duration-500 dark:text-slate-50 text-lg">
                  18-11-1842
                </p>
              </div>
            </div>
          </div>
          <div
            class="bg-slate-50 text-slate-500 transition-all duration-500 dark:bg-slate-600 transition-all duration-500 dark:text-slate-200 rounded-b-xl flex items-center">
            <div class="flex-auto flex items-center justify-evenly">
              <audio controls>
                <source src="Himnos/Beni.mp3" type="audio/mpeg">
                Tu navegador no admite la reproducción de audio.
              </audio>
            </div>
          </div>
        </div>
        <!-- fin reproductor -->

        <!-- reproductor -->
        <div class="mt-1 sm:mt-5 relative z-10 rounded-xl shadow-xl">
          <div
            class="bg-white border-slate-100 transition-all duration-500 dark:bg-slate-800 transition-all duration-500 dark:border-slate-500 border-b rounded-t-xl p-4 pb-6 sm:p-10 sm:pb-8 lg:p-6 xl:p-10 xl:pb-8 space-y-6 sm:space-y-8 lg:space-y-6 xl:space-y-8">
            <div class="flex items-center space-x-4">
              <img src="/img/Escudos/Litoral.gif" loading="lazy" decoding="async" alt=""
                class="flex-none rounded-lg bg-slate-100" width="88" height="88">
              <div class="min-w-0 flex-auto space-y-1 font-semibold">
                <p class="text-cyan-500 transition-all duration-500 dark:text-cyan-400 text-sm leading-6">
                  <abbr title="Episode">Dpto.</abbr> Beni
                </p>
                <h2 class="text-slate-500 transition-all duration-500 dark:text-slate-400 text-sm leading-6 truncate">
                  213.564 km²
                </h2>
                <p class="text-slate-900 transition-all duration-500 dark:text-slate-50 text-lg">
                  18-11-1842
                </p>
              </div>
            </div>
          </div>
          <div
            class="bg-slate-50 text-slate-500 transition-all duration-500 dark:bg-slate-600 transition-all duration-500 dark:text-slate-200 rounded-b-xl flex items-center">
            <div class="flex-auto flex items-center justify-evenly">
              <audio controls>
                <source src="Himnos/Beni.mp3" type="audio/mpeg">
                Tu navegador no admite la reproducción de audio.
              </audio>
            </div>
          </div>
        </div>
        <!-- fin reproductor -->
      </div>
    </div>

  </div>





  <!--Footer container-->
  

  
<footer class="bg-white rounded-lg shadow dark:bg-gray-900 m-4">
    <div class="w-full max-w-screen-xl mx-auto p-4 md:py-8">
        <div class="sm:flex sm:items-center sm:justify-between">
            <a href="https://flowbite.com/" class="flex items-center mb-4 sm:mb-0">
                <img src="https://www.svgrepo.com/show/405427/flag-for-flag-bolivia.svg" class="h-12 mr-3" alt="Flowbite Logo" />
                <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white">YovanEnovore</span>
            </a>
            <ul class="flex flex-wrap items-center mb-6 text-sm font-medium text-gray-500 sm:mb-0 dark:text-gray-400">
              <div class="container pt-9">
      <div class="mb-9 flex justify-center">
        <a href="https://www.facebook.com/ynvyvn/" class="mr-9 text-neutral-800 dark:text-neutral-200">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="currentColor" viewBox="0 0 24 24">
            <path
              d="M9 8h-3v4h3v12h5v-12h3.642l.358-4h-4v-1.667c0-.955.192-1.333 1.115-1.333h2.885v-5h-3.808c-3.596 0-5.192 1.583-5.192 4.615v3.385z" />
          </svg>
        </a>
        <a href="https://twitter.com/ramonenovore" class="mr-9 text-neutral-800 dark:text-neutral-200">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="currentColor" viewBox="0 0 24 24">
            <path
              d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z" />
          </svg>
        </a>
        <a href="https://www.instagram.com/ynvenovore/" class="mr-9 text-neutral-800 dark:text-neutral-200">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="currentColor" viewBox="0 0 24 24">
            <path
              d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z" />
          </svg>
        </a>
        <a href="https://www.linkedin.com/in/ynv-yovanramonyauneenovore/" class="mr-9 text-neutral-800 dark:text-neutral-200">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="currentColor" viewBox="0 0 24 24">
            <path
              d="M4.98 3.5c0 1.381-1.11 2.5-2.48 2.5s-2.48-1.119-2.48-2.5c0-1.38 1.11-2.5 2.48-2.5s2.48 1.12 2.48 2.5zm.02 4.5h-5v16h5v-16zm7.982 0h-4.968v16h4.969v-8.399c0-4.67 6.029-5.052 6.029 0v8.399h4.988v-10.131c0-7.88-8.922-7.593-11.018-3.714v-2.155z" />
          </svg>
        </a>
        <a href="https://github.com/ynvYauneEnovore" class="text-neutral-800 dark:text-neutral-200">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="currentColor" viewBox="0 0 24 24">
            <path
              d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z" />
          </svg>
        </a>
      </div>
    </div>
            </ul>
        </div>
        <hr class="my-6 border-gray-200 sm:mx-auto dark:border-gray-700 lg:my-8" />
        <span class="block text-sm text-gray-500 sm:text-center dark:text-gray-400">© 2023 <a href="https://yovanenovore.tech/" class="hover:underline">YovanEnovore™</a>. Todos los Derechos Reservados.</span>
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
