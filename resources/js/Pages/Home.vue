<template>
    <div>
        <div class="relative bg-white overflow-hidden">
            <div class="max-w-screen-xl mx-auto ">
                <div class="relative z-10 pb-8 bg-white sm:pb-16 md:pb-20 lg:max-w-2xl lg:w-full lg:pb-28 xl:pb-32">
                    <div class="pt-6 px-4 sm:px-6 lg:px-8">
                        <nav class="relative flex items-center justify-between sm:h-10 lg:justify-start">
                            <div class="flex items-center flex-grow flex-shrink-0 lg:flex-grow-0">
                                <div class="flex items-center justify-between w-full md:w-auto">
                                    <a href="#">
                                        <img class="h-8 w-auto sm:h-10"
                                             src="https://tailwindui.com/img/logos/workflow-mark-on-white.svg" alt=""/>
                                    </a>
                                    <div class="-mr-2 flex items-center md:hidden">
                                        <button @click="open = true" type="button"
                                                class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-500 transition duration-150 ease-in-out">
                                            <svg class="h-6 w-6" stroke="currentColor" fill="none" viewBox="0 0 24 24">
                                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                                      d="M4 6h16M4 12h16M4 18h16"/>
                                            </svg>
                                        </button>
                                    </div>
                                </div>
                            </div>
                            <div class="hidden md:block md:ml-10 md:pr-4">
                                <a href="#"
                                   class="font-medium text-gray-500 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out">Home</a>
                                <a href="#"
                                   class="ml-8 font-medium text-gray-500 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out">About</a>
                                <a href="#"
                                   class="ml-8 font-medium text-gray-500 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out">Vision</a>
                            </div>
                        </nav>
                    </div>

                    <div x-show="open" x-transition:enter="duration-150 ease-out"
                         x-transition:enter-start="opacity-0 scale-95" x-transition:enter-end="opacity-100 scale-100"
                         x-transition:leave="duration-100 ease-in" x-transition:leave-start="opacity-100 scale-100"
                         x-transition:leave-end="opacity-0 scale-95"
                         class="absolute top-0 inset-x-0 p-2 transition transform origin-top-right md:hidden">
                        <div class="rounded-lg shadow-md">
                            <div class="rounded-lg bg-white shadow-xs overflow-hidden">
                                <div class="px-5 pt-4 flex items-center justify-between">
                                    <div>
                                        <img class="h-8 w-auto" src="/img/logos/workflow-mark-on-white.svg" alt=""/>
                                    </div>
                                    <div class="-mr-2">
                                        <button @click="open = false" type="button"
                                                class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-500 transition duration-150 ease-in-out">
                                            <svg class="h-6 w-6" stroke="currentColor" fill="none" viewBox="0 0 24 24">
                                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                                      d="M6 18L18 6M6 6l12 12"/>
                                            </svg>
                                        </button>
                                    </div>
                                </div>
                                <div class="px-2 pt-2 pb-3">
                                    <a href="#"
                                       class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out">Product</a>
                                    <a href="#"
                                       class="mt-1 block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out">Features</a>
                                    <a href="#"
                                       class="mt-1 block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out">Marketplace</a>
                                    <a href="#"
                                       class="mt-1 block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out">Company</a>
                                </div>
                                <div>
                                    <a href="#"
                                       class="block w-full px-5 py-3 text-center font-medium text-indigo-600 bg-gray-50 hover:bg-gray-100 hover:text-indigo-700 focus:outline-none focus:bg-gray-100 focus:text-indigo-700 transition duration-150 ease-in-out">
                                        Log in
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="mt-10 mx-auto max-w-screen-xl px-4 sm:mt-12 sm:px-6 md:mt-16 lg:mt-20 lg:px-8 xl:mt-28">
                        <div class="sm:text-center lg:text-left">
                            <h2 class="text-4xl tracking-tight leading-10 font-extrabold text-gray-900 sm:text-5xl sm:leading-none md:text-6xl">
                                We brengen de kracht van technologie
                                <br class="xl:hidden"/>
                                <span class="text-indigo-600">naar politiek Nederland</span>
                            </h2>
                            <p class="mt-3 text-base text-gray-500 sm:mt-5 sm:text-lg sm:max-w-xl sm:mx-auto md:mt-5 md:text-xl lg:mx-0">
                                Het is tijd om het debat over te nemen van Den Haag.
                                Of je nu anoniem wilt blijven of niet, het is nu mogelijk om je mening uit te spreken samen met andere like-minded Nederlanders.
                            </p>
                            <div class="mt-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
                                <div class="rounded-md shadow">
                                    <a href="#"
                                       class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base leading-6 font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-500 focus:outline-none focus:shadow-outline transition duration-150 ease-in-out md:py-4 md:text-lg md:px-10">
                                        Ga het gesprek aan
                                    </a>
                                </div>
                                <div class="mt-3 sm:mt-0 sm:ml-3">
                                    <a href="#"
                                       class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base leading-6 font-medium rounded-md text-indigo-700 bg-indigo-100 hover:text-indigo-600 hover:bg-indigo-50 focus:outline-none focus:shadow-outline focus:border-indigo-300 transition duration-150 ease-in-out md:py-4 md:text-lg md:px-10">
                                        Lees meer
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>
                    <svg
                        class="hidden lg:block absolute right-0 inset-y-0 h-full w-48 text-white transform translate-x-1/2"
                        fill="currentColor" viewBox="0 0 100 100" preserveAspectRatio="none">
                        <polygon points="50,0 100,0 50,100 0,100"/>
                    </svg>
                </div>
            </div>
            <div class="lg:absolute lg:inset-y-0 lg:right-0 lg:w-1/2">
                <img class="h-56 w-full object-cover sm:h-72 md:h-96 lg:w-full lg:h-full"
                     src="https://images.nrc.nl/RyBudRGwkIr_jb4IlN9GkvulXMg=/1280x/filters:no_upscale()/s3/static.nrc.nl/wp-content/uploads/2018/03/web-2203bintk.jpg.jpg"
                     alt=""/>
            </div>
        </div>
        <div class="py-12 bg-white">
            <div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="lg:text-center">
                    <p class="text-base leading-6 text-indigo-600 font-semibold tracking-wide uppercase">
                        Online Discussie</p>
                    <h3 class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl sm:leading-10">
                        Een betere manier om politiek te bespreken, met iedereen.
                    </h3>
                    <p class="mt-4 max-w-2xl text-xl leading-7 text-gray-500 lg:mx-auto">
                        DING is een volksvergadering dat afstand uit de oud-Germaanse tijd. Hierin werd rechtgesproken door de aanwezigen in die vergadering.
                        Hieronder lees je enkele eigenschappen van DING. Onze beloftes aan jou.
                    </p>
                </div>

                <div class="mt-10">
                    <ul class="md:grid md:grid-cols-2 md:col-gap-8 md:row-gap-10">
                        <li>
                            <div class="flex">
                                <div class="flex-shrink-0">
                                    <div
                                        class="flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white">
                                        <svg class="h-6 w-6" stroke="currentColor" fill="none" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                                  d="M21 12a9 9 0 01-9 9m9-9a9 9 0 00-9-9m9 9H3m9 9a9 9 0 01-9-9m9 9c1.657 0 3-4.03 3-9s-1.343-9-3-9m0 18c-1.657 0-3-4.03-3-9s1.343-9 3-9m-9 9a9 9 0 019-9"/>
                                        </svg>
                                    </div>
                                </div>
                                <div class="ml-4">
                                    <h5 class="text-lg leading-6 font-medium text-gray-900">Verschillende kamers voor verschillende onderwerpen</h5>
                                    <p class="mt-2 text-base leading-6 text-gray-500">
                                        Of je nu over COVID-19 wilt spreken of over de manier hoe de overheid privé API’s gebruikt om stoplichten aan te sturen, er is voor elk onderwerp een kamer.
                                        Is er geen kamer voor het onderwerp wat jij wilt bespreken? Dan kun je een nieuwe kamer aanmaken.
                                    </p>
                                </div>
                            </div>
                        </li>
                        <li class="mt-10 md:mt-0">
                            <div class="flex">
                                <div class="flex-shrink-0">
                                    <div
                                        class="flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white">
                                        <svg class="h-6 w-6" stroke="currentColor" fill="none" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                                  d="M3 6l3 1m0 0l-3 9a5.002 5.002 0 006.001 0M6 7l3 9M6 7l6-2m6 2l3-1m-3 1l-3 9a5.002 5.002 0 006.001 0M18 7l3 9m-3-9l-6-2m0-2v2m0 16V5m0 16H9m3 0h3"/>
                                        </svg>
                                    </div>
                                </div>
                                <div class="ml-4">
                                    <h5 class="text-lg leading-6 font-medium text-gray-900">Politiek profiel</h5>
                                    <p class="mt-2 text-base leading-6 text-gray-500">
                                        Om ons DING te gebruiken, zul je een politiek profiel moeten aanmaken.
                                        Dit is zodat andere gebruikers beter kunnen begrijpen waar jouw meningen op gebaseerd zijn.
                                    </p>
                                </div>
                            </div>
                        </li>
                        <li class="mt-10 md:mt-0">
                            <div class="flex">
                                <div class="flex-shrink-0">
                                    <div
                                        class="flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white">
                                        <svg class="h-6 w-6" stroke="currentColor" fill="none" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                                  d="M13 10V3L4 14h7v7l9-11h-7z"/>
                                        </svg>
                                    </div>
                                </div>
                                <div class="ml-4">
                                    <h5 class="text-lg leading-6 font-medium text-gray-900">Compleet gratis</h5>
                                    <p class="mt-2 text-base leading-6 text-gray-500">
                                        Vrijheid van meningsuiting is niet gereserveerd voor de politici in Den Haag. Het is vrij voor iedereen.
                                        Daarom is ons platform kosteloos.
                                    </p>
                                </div>
                            </div>
                        </li>
                        <li class="mt-10 md:mt-0">
                            <div class="flex">
                                <div class="flex-shrink-0">
                                    <div
                                        class="flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white">
                                        <svg class="h-6 w-6" stroke="currentColor" fill="none" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                                  d="M7 8h10M7 12h4m1 8l-4-4H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-3l-4 4z"/>
                                        </svg>
                                    </div>
                                </div>
                                <div class="ml-4">
                                    <h5 class="text-lg leading-6 font-medium text-gray-900">Progressief, ook in onze technologie.</h5>
                                    <p class="mt-2 text-base leading-6 text-gray-500">
                                        Een fysieke installatie is beschikbaar naast de Markthal in Rotterdam. In deze installatie wordt het debat aangegaan. Om dit openbaar voor iedereen te maken wordt dit live uitgezonden. Je privacy is erg belangrijk voor ons, daarom wordt je gezicht niet uitgezonden en wordt je stem vervormd. Enkel je avatar is zichtbaar.
                                        Om ervoor te zorgen dat iedereen gebruik kan maken van ons platform, kun je het op elk apparaat gebruiken. Of het nu een laptop of een telefoon is, er is altijd een mogelijkheid om je mening te delen. Geen excuusjes meer om de discussie niet aan te gaan.
                                    </p>
                                </div>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Home"
    }
</script>

<style scoped>

</style>
