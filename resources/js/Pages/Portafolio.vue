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
    <Head title="Hi" />
    <!-- component -->
    <div class="bg-white">
        <div class="container m-auto px-6 text-gray-600 md:px-12 xl:px-6">
            <div
                class="space-y-6 md:space-y-0 md:flex md:gap-6 lg:items-center lg:gap-12"
            >
                <div class="md:5/12 lg:w-5/12">
                    <img
                        src="/img/1.png"
                        alt="image"
                        loading="lazy"
                        width="350"
                        height=""
                    />
                </div>
                <div class="md:7/12 lg:w-6/12">
                    <h2 class="text-2xl text-gray-900 font-bold md:text-4xl">
                        Technology enthusiast 💻
                    </h2>
                    <p class="mt-6 text-gray-600">
I'm Yovan, a passionate Full Stack developer with a strong focus on backend development. I have extensive experience building robust and scalable web applications from scratch. My main experience lies in designing and developing the logic and databases that drive applications, ensuring optimal performance and strong security. Furthermore, I am deeply committed to excellence and continuous improvement in the field of information technology.
                    </p>
                </div>
            </div>
        </div>
    </div>

    <!-- component -->
    <div class="h-screen flex items-center justify-center">
        <card class="relative h-[30rem] sm:h-96 w-[35rem] rounded-lg">
            <!-- Background Image -->
            <img
                src="https://picsum.photos/seed/1840/1000/600"
                class="object-cover w-full h-full rounded-lg"
            />

            <!-- Content -->
            <div
                class="absolute w-full h-full bottom-0 bg-gradient-to-r from-fuchsia-700/30 to-violet-700 rounded-lg flex flex-col items-center justify-center text-center"
            >
                <!-- Company Logo -->
                <svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="400"
                    height="100"
                >
                    <text
                        x="20"
                        y="80"
                        font-family="Arial"
                        font-size="40"
                        fill="white"
                    >
                        Yovan
                    </text>
                </svg>

                <!-- Quotes -->
                <p class="text-lg px-14 text-gray-300 mt-5">
                    Soy un desarrollador web y de aplicaciones que garantiza su
                    funcionamiento y apariencia, tanto en la parte visible como
                    en la invisible. Mi objetivo es hacer que todo funcione sin
                    problemas en línea.
                </p>

                <!-- Photo -->
                <img
                    src="https://secure.gravatar.com/avatar/307f127a06b20c136e863f585a41f548?s=800&d=identicon"
                    class="rounded-full border-2 mt-8"
                    width="50"
                />

                <!-- Title -->
                <p class="text-base font-bold px-14 text-gray-300 mt-3">
                    Desarrollador de Sistemas Informáticos Multiplataforma
                </p>

                <p class="text-sm font-light px-14 text-gray-300">
                    yovanenovore
                </p>
            </div>
        </card>
    </div>

    <!-- component -->
    <div class="h-screen flex items-center justify-center bg-amber-50">
        <div class="grid grid-cols-6 gap-x-4 gap-y-1 max-w-2xl">
            <!-- Title -->
            <div class="col-span-full mb-3">
                <p class="text-xl text-gray-800 font-bold">
                    HABILIDADES DESTACADAS
                </p>
            </div>

            <!-- Card 1 -->
            <div class="col-span-2">
                <a href="">
                    <img
                        src="https://www.svgrepo.com/show/452192/docker.svg"
                        class="rounded-xl"
                    />
                </a>
            </div>

            <!-- Card 2 -->
            <div class="col-span-2">
                <a href="">
                    <img
                        src="https://www.svgrepo.com/show/452210/git.svg"
                        class="rounded-xl"
                    />
                </a>
            </div>

            <!-- Card 3 -->
            <div class="col-span-2">
                <a href="">
                    <img
                        src="https://www.svgrepo.com/show/353985/laravel.svg"
                        class="rounded-xl"
                    />
                </a>
            </div>

            <!-- Card 4 -->
            <div class="col-span-2">
                <a href="">
                    <img
                        src="https://www.svgrepo.com/show/452184/csharp.svg"
                        class="rounded-xl"
                    />
                </a>
            </div>

            <!-- Card 5 -->
            <div class="col-span-2">
                <a href="">
                    <img
                        src="https://www.svgrepo.com/show/448236/linux.svg"
                        class="rounded-xl"
                    />
                </a>
            </div>

            <!-- Card 5 -->
            <div class="col-span-2">
                <a href="">
                    <img
                        src="https://www.svgrepo.com/show/530439/api-interface.svg"
                        class="rounded-xl"
                    />
                </a>
            </div>
        </div>
    </div>

    <div
        class="fixed z-50 w-full h-16 max-w-lg -translate-x-1/2 bg-white border border-gray-200 rounded-full bottom-4 left-1/2 dark:bg-gray-700 dark:border-gray-600"
    >
        <div class="grid h-full max-w-lg grid-cols-5 mx-auto">
            <a
                data-tooltip-target="tooltip-home"
                type="button"
                class="inline-flex flex-col items-center justify-center px-5 rounded-l-full hover:bg-gray-50 dark:hover:bg-gray-800 group"
                href="/"
            >
                <svg
                    class="w-5 h-5 mb-1 text-gray-500 dark:text-gray-400 group-hover:text-blue-600 dark:group-hover:text-blue-500"
                    aria-hidden="true"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="currentColor"
                    viewBox="0 0 20 20"
                >
                    <path
                        d="m19.707 9.293-2-2-7-7a1 1 0 0 0-1.414 0l-7 7-2 2a1 1 0 0 0 1.414 1.414L2 10.414V18a2 2 0 0 0 2 2h3a1 1 0 0 0 1-1v-4a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1v4a1 1 0 0 0 1 1h3a2 2 0 0 0 2-2v-7.586l.293.293a1 1 0 0 0 1.414-1.414Z"
                    />
                </svg>
                <span class="sr-only">Home</span>
            </a>
            <div
                id="tooltip-home"
                role="tooltip"
                class="absolute z-10 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700"
            >
                Home
                <div class="tooltip-arrow" data-popper-arrow></div>
            </div>
            <button
            
                data-tooltip-target="tooltip-wallet"
                type="button"
                class="inline-flex flex-col items-center justify-center px-5 hover:bg-gray-50 dark:hover:bg-gray-800 group"
            >
                <svg
                    class="w-5 h-5 mb-1 text-gray-500 dark:text-gray-400 group-hover:text-blue-600 dark:group-hover:text-blue-500"
                    aria-hidden="true"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="currentColor"
                    viewBox="0 0 20 20"
                >
                    <path
                        d="M11.074 4 8.442.408A.95.95 0 0 0 7.014.254L2.926 4h8.148ZM9 13v-1a4 4 0 0 1 4-4h6V6a1 1 0 0 0-1-1H1a1 1 0 0 0-1 1v13a1 1 0 0 0 1 1h17a1 1 0 0 0 1-1v-2h-6a4 4 0 0 1-4-4Z"
                    />
                    <path
                        d="M19 10h-6a2 2 0 0 0-2 2v1a2 2 0 0 0 2 2h6a1 1 0 0 0 1-1v-3a1 1 0 0 0-1-1Zm-4.5 3.5a1 1 0 1 1 0-2 1 1 0 0 1 0 2ZM12.62 4h2.78L12.539.41a1.086 1.086 0 1 0-1.7 1.352L12.62 4Z"
                    />
                </svg>
                <span class="sr-only">Wallet</span>
            </button>
            <div
                id="tooltip-wallet"
                role="tooltip"
                class="absolute z-10 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700"
            >
                Wallet
                <div class="tooltip-arrow" data-popper-arrow></div>
            </div>
            <div class="flex items-center justify-center">
                <button
                    data-tooltip-target="tooltip-new"
                    type="button"
                    class="inline-flex items-center justify-center w-10 h-10 font-medium bg-blue-600 rounded-full hover:bg-blue-700 group focus:ring-4 focus:ring-blue-300 focus:outline-none dark:focus:ring-blue-800"
                >
                    <svg
                        class="w-4 h-4 text-white"
                        aria-hidden="true"
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 18 18"
                    >
                        <path
                            stroke="currentColor"
                            stroke-linecap="round"
                            stroke-linejoin="round"
                            stroke-width="2"
                            d="M9 1v16M1 9h16"
                        />
                    </svg>
                    <span class="sr-only">New item</span>
                </button>
            </div>
            <div
                id="tooltip-new"
                role="tooltip"
                class="absolute z-10 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700"
            >
                Create new item
                <div class="tooltip-arrow" data-popper-arrow></div>
            </div>
            <button
                data-tooltip-target="tooltip-settings"
                type="button"
                class="inline-flex flex-col items-center justify-center px-5 hover:bg-gray-50 dark:hover:bg-gray-800 group"
            >
                <svg
                    class="w-5 h-5 mb-1 text-gray-500 dark:text-gray-400 group-hover:text-blue-600 dark:group-hover:text-blue-500"
                    aria-hidden="true"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 20 20"
                >
                    <path
                        stroke="currentColor"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                        stroke-width="2"
                        d="M4 12.25V1m0 11.25a2.25 2.25 0 0 0 0 4.5m0-4.5a2.25 2.25 0 0 1 0 4.5M4 19v-2.25m6-13.5V1m0 2.25a2.25 2.25 0 0 0 0 4.5m0-4.5a2.25 2.25 0 0 1 0 4.5M10 19V7.75m6 4.5V1m0 11.25a2.25 2.25 0 1 0 0 4.5 2.25 2.25 0 0 0 0-4.5ZM16 19v-2"
                    />
                </svg>
                <span class="sr-only">Settings</span>
            </button>
            <div
                id="tooltip-settings"
                role="tooltip"
                class="absolute z-10 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700"
            >
                Settings
                <div class="tooltip-arrow" data-popper-arrow></div>
            </div>
            <button
                data-tooltip-target="tooltip-profile"
                type="button"
                class="inline-flex flex-col items-center justify-center px-5 rounded-r-full hover:bg-gray-50 dark:hover:bg-gray-800 group"
            >
                <svg
                    class="w-5 h-5 mb-1 text-gray-500 dark:text-gray-400 group-hover:text-blue-600 dark:group-hover:text-blue-500"
                    aria-hidden="true"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="currentColor"
                    viewBox="0 0 20 20"
                >
                    <path
                        d="M10 0a10 10 0 1 0 10 10A10.011 10.011 0 0 0 10 0Zm0 5a3 3 0 1 1 0 6 3 3 0 0 1 0-6Zm0 13a8.949 8.949 0 0 1-4.951-1.488A3.987 3.987 0 0 1 9 13h2a3.987 3.987 0 0 1 3.951 3.512A8.949 8.949 0 0 1 10 18Z"
                    />
                </svg>
                <span class="sr-only">Profile</span>
            </button>
            <div
                id="tooltip-profile"
                role="tooltip"
                class="absolute z-10 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700"
            >
                Profile
                <div class="tooltip-arrow" data-popper-arrow></div>
            </div>
        </div>
    </div>

    <!-- Componente Footer -->
    <footer class="bg-gradient-to-r from-gray-100 via-[#bce1ff] to-gray-100">
        <div class="max-w-screen-xl px-4 py-16 mx-auto sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 gap-8 lg:grid-cols-3">
                <!-- Sección de información de la empresa -->
                <div>
                    <img src="https://raw.githubusercontent.com/ynvYauneEnovore/personal-port/main/public/img/ynv.png" class="mr-5 h-6 sm:h-9" alt="logo" />
                    <p class="max-w-xs mt-4 text-sm text-gray-600">
                      Transforma tus sueños digitales en realidad. Como desarrollador Full Stack, estoy listo para dar vida a tus ideas desde todos los ángulos.
                    </p>
                    <div class="flex mt-8 space-x-6 text-gray-600">
                        <!-- Enlaces a redes sociales -->
                        <a
                            class="hover:opacity-75"
                            href="#"
                            target="_blank"
                            rel="noreferrer"
                        >

                                   <img
                        src="https://secure.gravatar.com/avatar/307f127a06b20c136e863f585a41f548?s=800&d=identicon"
                        alt="image"
                        loading="lazy"
                        width="100"
                        height=""
                    />
                        </a>
                        <a
                            class="hover:opacity-75"
                            href="#"
                            target="_blank"
                            rel="noreferrer"
                        >
                            <span class="sr-only"> Instagram </span>
                            <!-- Ícono de Instagram -->
                        </a>
                        <a
                            class="hover:opacity-75"
                            href="#"
                            target="_blank"
                            rel="noreferrer"
                        >
                            <span class="sr-only"> Twitter </span>
                            <!-- Ícono de Twitter -->
                        </a>
                        <a
                            class="hover:opacity-75"
                            href="#"
                            target="_blank"
                            rel="noreferrer"
                        >
                            <span class="sr-only"> GitHub </span>
                            <!-- Ícono de GitHub -->
                        </a>
                        <a
                            class="hover:opacity-75"
                            href="#"
                            target="_blank"
                            rel="noreferrer"
                        >
                            <span class="sr-only"> Dribbble </span>
                            <!-- Ícono de Dribbble -->
                        </a>
                    </div>
                </div>
                <!-- Sección de enlaces de navegación -->
                <div
                    class="grid grid-cols-1 gap-8 lg:col-span-2 sm:grid-cols-2 lg:grid-cols-4"
                >
                    <!-- Enlaces relacionados con la empresa -->
                    <div>
                        <p class="font-medium">Empresa</p>
                        <nav
                            class="flex flex-col mt-4 space-y-2 text-sm text-gray-500"
                        >
                            <a class="hover:opacity-75" href="https://ogymsa1.clubspazio.com/login"> Acerca de </a>
                           
                        </nav>
                    </div>
                    <!-- Enlaces de servicios ofrecidos -->
                    <div>
                        <p class="font-medium">Servicios</p>
                        <nav
                            class="flex flex-col mt-4 space-y-2 text-sm text-gray-500"
                        >
                            <a class="hover:opacity-75" href="https://yovanenovore.tech">
                                Optimización de SEO
                            </a>
                        </nav>
                    </div>
                    <!-- Enlaces útiles -->
                    <div>
                        <p class="font-medium">Enlaces Útiles</p>
                        <nav
                            class="flex flex-col mt-4 space-y-2 text-sm text-gray-500"
                        >
                        <a class="hover:opacity-75" href="https://yovanenovore.tech">
                                deb FULL STACK
                            </a>
                        </nav>
                    </div>
                    <!-- Enlaces legales -->
                    <div>
                        <p class="font-medium">Legal</p>
                        <nav
                            class="flex flex-col mt-4 space-y-2 text-sm text-gray-500"
                        >
                            <a class="hover:opacity-75" href="https://yovanenovore.tech">
                                Política de Privacidad
                            </a>
                         
                        </nav>
                    </div>
                </div>
            </div>
            <!-- Aviso de derechos de autor -->
            <p class="mt-8 text-xs text-gray-800">
                Todo los Derechos Reservados © 2023 yovanenovore
            </p>
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
