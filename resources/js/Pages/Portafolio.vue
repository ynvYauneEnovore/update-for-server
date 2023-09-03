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
    <div class="py-16 bg-white">
        <div class="container m-auto px-6 text-gray-600 md:px-12 xl:px-6">
            <div
                class="space-y-6 md:space-y-0 md:flex md:gap-6 lg:items-center lg:gap-12"
            >
                <div class="md:5/12 lg:w-5/12">
                    <img
                        src="https://secure.gravatar.com/avatar/307f127a06b20c136e863f585a41f548?s=800&d=identicon"
                        alt="image"
                        loading="lazy"
                        width="400"
                        height=""
                    />
                </div>
                <div class="md:7/12 lg:w-6/12">
                    <h2 class="text-2xl text-gray-900 font-bold md:text-4xl">
                        Amante de la tecnología 💻
                    </h2>
                    <p class="mt-6 text-gray-600">
                        Soy Yovan, un apasionado desarrollador Full Stack con un
                        enfoque sólido en el desarrollo backend. Tengo una
                        amplia experiencia en la creación de aplicaciones web
                        robustas y escalables desde cero. Mi habilidad principal
                        radica en diseñar y desarrollar las lógicas y bases de
                        datos que hacen funcionar las aplicaciones, garantizando
                        un rendimiento óptimo y una seguridad sólida. Además,
                        tengo un firme compromiso con la excelencia y la mejora
                        continua en el campo del desarrollo web.
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
                        Yovan Ramón
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
                    Yovan Ramón
                </p>
            </div>
        </card>
    </div>
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
