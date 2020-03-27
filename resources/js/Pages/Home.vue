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
                                        <img alt=""
                                             class="h-8 w-auto sm:h-10" src="/images/Ding_Concept_Logo.svg"/>
                                    </a>
                                    <div class="-mr-2 flex items-center md:hidden">
                                        <button @click="open = true"
                                                class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-500 transition duration-150 ease-in-out"
                                                type="button">
                                            <svg class="h-6 w-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                                <path d="M4 6h16M4 12h16M4 18h16" stroke-linecap="round"
                                                      stroke-linejoin="round"
                                                      stroke-width="2"/>
                                            </svg>
                                        </button>
                                    </div>
                                </div>
                            </div>
                            <div class="hidden md:block md:ml-10 md:pr-4" style="display:none;">
                                <a class="font-medium text-gray-500 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out"
                                   href="#">Home</a>
                                <a class="ml-8 font-medium text-gray-500 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out"
                                   href="#">About</a>
                                <a class="ml-8 font-medium text-gray-500 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out"
                                   href="#">Vision</a>
                            </div>
                        </nav>
                    </div>

                    <div class="absolute top-0 inset-x-0 p-2 transition transform origin-top-right md:hidden"
                         x-show="open"
                         x-transition:enter="duration-150 ease-out" x-transition:enter-end="opacity-100 scale-100"
                         x-transition:enter-start="opacity-0 scale-95" x-transition:leave="duration-100 ease-in"
                         x-transition:leave-end="opacity-0 scale-95"
                         x-transition:leave-start="opacity-100 scale-100">
                        <div class="rounded-lg shadow-md">
                            <div class="rounded-lg bg-white shadow-xs overflow-hidden">
                                <div class="px-5 pt-4 flex items-center justify-between">
                                    <div>
                                        <img alt="" class="h-8 w-auto" src="/img/logos/workflow-mark-on-white.svg"/>
                                    </div>
                                    <div class="-mr-2">
                                        <button @click="open = false"
                                                class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-500 transition duration-150 ease-in-out"
                                                type="button">
                                            <svg class="h-6 w-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                                <path d="M6 18L18 6M6 6l12 12" stroke-linecap="round"
                                                      stroke-linejoin="round"
                                                      stroke-width="2"/>
                                            </svg>
                                        </button>
                                    </div>
                                </div>
                                <div class="px-2 pt-2 pb-3">
                                    <a class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out"
                                       href="#">Product</a>
                                    <a class="mt-1 block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out"
                                       href="#">Features</a>
                                    <a class="mt-1 block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out"
                                       href="#">Marketplace</a>
                                    <a class="mt-1 block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out"
                                       href="#">Company</a>
                                </div>
                                <div>
                                    <a class="block w-full px-5 py-3 text-center font-medium text-indigo-600 bg-gray-50 hover:bg-gray-100 hover:text-indigo-700 focus:outline-none focus:bg-gray-100 focus:text-indigo-700 transition duration-150 ease-in-out"
                                       href="#">
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
                                In dit project zoeken we uit hoe wij jongeren bewust(er) kunnen maken van social
                                cooling. Dit proberen wij te realiseren door een concept uit te werken genaamd DING.
                            </p>
                            <div class="mt-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
                                <div class="rounded-md shadow">
                                    <a class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base leading-6 font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-500 focus:outline-none focus:shadow-outline transition duration-150 ease-in-out md:py-4 md:text-lg md:px-10"
                                       href="#">
                                        Ga het gesprek aan
                                    </a>
                                </div>
                                <div class="mt-3 sm:mt-0 sm:ml-3">
                                    <a class="w-full flex items-center justify-center px-8 py-3 border border-transparent text-base leading-6 font-medium rounded-md text-indigo-700 bg-indigo-100 hover:text-indigo-600 hover:bg-indigo-50 focus:outline-none focus:shadow-outline focus:border-indigo-300 transition duration-150 ease-in-out md:py-4 md:text-lg md:px-10"
                                       href="#onsteam">
                                        Ons Team
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>
                    <svg
                        class="hidden lg:block absolute right-0 inset-y-0 h-full w-48 text-white transform translate-x-1/2"
                        fill="currentColor" preserveAspectRatio="none" viewBox="0 0 100 100">
                        <polygon points="50,0 100,0 50,100 0,100"/>
                    </svg>
                </div>
            </div>
            <div class="lg:absolute lg:inset-y-0 lg:right-0 lg:w-1/2">
                <img alt=""
                     class="h-56 w-full object-cover sm:h-72 md:h-96 lg:w-full lg:h-full"
                     src="https://images.nrc.nl/RyBudRGwkIr_jb4IlN9GkvulXMg=/1280x/filters:no_upscale()/s3/static.nrc.nl/wp-content/uploads/2018/03/web-2203bintk.jpg.jpg"/>
            </div>
        </div>
        <br>
        <br>
        <br>
        <br>
        <br>
        <div class="py-12 bg-white">
            <div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="lg:text-center">
                    <p class="text-base leading-6 text-indigo-600 font-semibold tracking-wide uppercase">
                        Online Debat</p>
                    <h3 class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl sm:leading-10">
                        Een betere manier om politiek te bespreken, met iedereen.
                    </h3>
                    <p class="mt-4 max-w-2xl text-xl leading-7 text-gray-500 lg:mx-auto">
                        DING is een volksvergadering dat afstand uit de oud-Germaanse tijd. Hierin werd rechtgesproken
                        door de aanwezigen in die vergadering.
                        Hieronder lees je enkele eigenschappen van DING. Onze beloftes aan jou.
                    </p>
                </div>
                <br>
                <br>
                <br>
                <br>
                <br>
                <div class="mt-10">
                    <ul class="md:grid md:grid-cols-2 md:col-gap-8 md:row-gap-10">
                        <li>
                            <div class="flex">
                                <div class="flex-shrink-0">
                                    <div
                                        class="flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white">
                                        <svg class="h-6 w-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path
                                                d="M7 8h10M7 12h4m1 8l-4-4H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-3l-4 4z"
                                                stroke-linecap="round" stroke-linejoin="round"
                                                stroke-width="2"/>
                                        </svg>
                                    </div>
                                </div>
                                <div class="ml-4">
                                    <h5 class="text-lg leading-6 font-medium text-gray-900">Verschillende kamers voor
                                        verschillende onderwerpen</h5>
                                    <p class="mt-2 text-base leading-6 text-gray-500">
                                        Of je nu over COVID-19 wilt spreken of over de manier hoe de overheid privé
                                        API’s gebruikt om stoplichten aan te sturen, er is voor elk onderwerp een kamer.
                                        Is er geen kamer voor het onderwerp wat jij wilt bespreken? Dan kun je een
                                        nieuwe kamer aanmaken.
                                    </p>
                                </div>
                            </div>
                        </li>
                        <li class="mt-10 md:mt-0">
                            <div class="flex">
                                <div class="flex-shrink-0">
                                    <div
                                        class="flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white">
                                        <svg class="h-6 w-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path
                                                d="M3 6l3 1m0 0l-3 9a5.002 5.002 0 006.001 0M6 7l3 9M6 7l6-2m6 2l3-1m-3 1l-3 9a5.002 5.002 0 006.001 0M18 7l3 9m-3-9l-6-2m0-2v2m0 16V5m0 16H9m3 0h3"
                                                stroke-linecap="round" stroke-linejoin="round"
                                                stroke-width="2"/>
                                        </svg>
                                    </div>
                                </div>
                                <div class="ml-4">
                                    <h5 class="text-lg leading-6 font-medium text-gray-900">Politiek profiel</h5>
                                    <p class="mt-2 text-base leading-6 text-gray-500">
                                        Om ons DING te gebruiken, zul je een politiek profiel moeten aanmaken.
                                        Dit is zodat andere gebruikers beter kunnen begrijpen waar jouw meningen op
                                        gebaseerd zijn.
                                    </p>
                                </div>
                            </div>
                        </li>
                        <li class="mt-10 md:mt-0">
                            <div class="flex">
                                <div class="flex-shrink-0">
                                    <div
                                        class="flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white">
                                        <svg class="h-6 w-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path d="M13 10V3L4 14h7v7l9-11h-7z" stroke-linecap="round"
                                                  stroke-linejoin="round"
                                                  stroke-width="2"/>
                                        </svg>
                                    </div>
                                </div>
                                <div class="ml-4">
                                    <h5 class="text-lg leading-6 font-medium text-gray-900">Compleet gratis</h5>
                                    <p class="mt-2 text-base leading-6 text-gray-500">
                                        Vrijheid van meningsuiting is niet gereserveerd voor de politici in Den Haag.
                                        Het is vrij voor iedereen.
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
                                        <svg class="h-6 w-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path
                                                d="M21 12a9 9 0 01-9 9m9-9a9 9 0 00-9-9m9 9H3m9 9a9 9 0 01-9-9m9 9c1.657 0 3-4.03 3-9s-1.343-9-3-9m0 18c-1.657 0-3-4.03-3-9s1.343-9 3-9m-9 9a9 9 0 019-9"
                                                stroke-linecap="round" stroke-linejoin="round"
                                                stroke-width="2"/>
                                        </svg>
                                    </div>
                                </div>
                                <div class="ml-4">
                                    <h5 class="text-lg leading-6 font-medium text-gray-900">Progressief, ook in onze
                                        technologie.</h5>
                                    <p class="mt-2 text-base leading-6 text-gray-500">
                                        Een fysieke installatie is beschikbaar naast de Markthal in Rotterdam. In deze
                                        installatie wordt het debat aangegaan. Om dit openbaar voor iedereen te maken
                                        wordt dit live uitgezonden. Je privacy is erg belangrijk voor ons, daarom wordt
                                        je gezicht niet uitgezonden en wordt je stem vervormd. Enkel je avatar is
                                        zichtbaar.
                                        Om ervoor te zorgen dat iedereen gebruik kan maken van ons platform, kun je het
                                        op elk apparaat gebruiken. Of het nu een laptop of een telefoon is, er is altijd
                                        een mogelijkheid om je mening te delen. Geen excuusjes meer om de discussie niet
                                        aan te gaan.
                                    </p>
                                </div>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <br>
        <br>
        <embed src="/pdf/poster.pdf" type="application/pdf" width="100%" height="1700px">
        <div class="py-12 bg-blackblack">
            <div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="lg:text-center" id="onsteam">
                    <h3 class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-white sm:text-4xl sm:leading-10">
                        Wij zijn team Normalin
                    </h3>
                    <p class="mt-4 max-w-2xl text-xl leading-7 text-gray-500 lg:mx-auto">
                        Wij zijn een jong team bestaande uit vijf personen, en willen zorgen voor een bewustere online
                        gedachtengang vooral gericht op jongeren.
                    </p>
                </div>
                <br>
                <br>
                <br>
                <div>
                    <img src="/images/team.png"/>
                </div>
                <br>
                <br>
                <br>
                <br>
                <br>
                <div class="mt-10">

                </div>
            </div>
        </div>
        <div class="py-12 bg-blackblack">
            <div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="lg:text-center" id="onsteam">
                    <h3 class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-white sm:text-4xl sm:leading-10">
                        Onderzoek
                    </h3>
                    <p class="mt-4 max-w-2xl text-xl leading-7 text-gray-500 lg:mx-auto">
                        Hoe kunnen we jongeren bewust maken over privacyrisico's?
                    </p>
                    <br>


                            <div class="flex flex-wrap text-white text-center text-2xl my-2">
                            <div class="w-1/2 my-2">
                            Gedragen jongeren zich anders online?
                            </div>
                                <div class="w-1/2 my-2">
                            Waar denken jongeren aan bij termen zoals Social Cooling & Chilling Effect?
                                </div>  <div class="w-1/2 my-2">
                            Wat denken de jongeren dat het effect is van social cooling?
                            </div>     <div class="w-1/2 my-2">
                            Hoe denken jongeren dat hun eigen kinderen om zullen gaan met online bezigheden?

                            </div></div>
                </div>
   <div class="text-center text-xl text-white mt-24 italic">"Veel jongeren willen de controle over hun persoonsgegevens dus wel in eigen handen nemen om
       baas te blijven over hun online imago, maar zijn op institutioneel niveau, bijv. in het controleren of
       voorkomen van de ‘schimmige’ kanten van datamining, minder daadkrachtig."</div>

            </div>
        </div>
        <div class="py-12 bg-blackblack">
            <div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="lg:text-center" id="onsteam">
                    <h3 class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-white sm:text-4xl sm:leading-10">
                        Insights
                    </h3>
                    <div class="flex flex-wrap">
                        <div class="w-1/2">
                    <div class="max-w-md py-4 px-8 bg-white shadow-lg rounded-lg my-20">
                        <div class="flex justify-center md:justify-end -mt-16">
                            <img class="w-20 h-20 object-cover rounded-full border-2 border-indigo-500" src="https://images.unsplash.com/photo-1520697830682-bbb6e85e2b0b?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=334&q=80">
                        </div>
                        <div>
                            <h2 class="text-gray-800 text-3xl font-semibold">Privacy</h2>
                        </div>
                        <div class="flex justify-end mt-4">

                        </div>
                    </div>

                    <div class="max-w-md py-4 px-8 bg-white shadow-lg rounded-lg my-20">
                        <div class="flex justify-center md:justify-end -mt-16">
                            <img class="w-20 h-20 object-cover rounded-full border-2 border-indigo-500" src="https://images.unsplash.com/photo-1522087066130-0c8c39bb0558?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=334&q=80">
                        </div>
                        <div>
                            <h2 class="text-gray-800 text-3xl font-semibold">Impactvol</h2>
                        </div>
                        <div class="flex justify-end mt-4">

                        </div>
                    </div>
                        </div>
                        <div class="w-1/2">
                    <div class="max-w-md py-4 px-8 bg-white shadow-lg rounded-lg my-20">
                        <div class="flex justify-center md:justify-end -mt-16">
                            <img class="w-20 h-20 object-cover rounded-full border-2 border-indigo-500" src="https://images.unsplash.com/photo-1499714608240-22fc6ad53fb2?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=334&q=80">
                        </div>
                        <div>
                            <h2 class="text-gray-800 text-3xl font-semibold">Bewustwoording</h2>
                        </div>
                        <div class="flex justify-end mt-4">

                        </div>
                    </div>

                    <div class="max-w-md py-4 px-8 bg-white shadow-lg rounded-lg my-20">
                        <div class="flex justify-center md:justify-end -mt-16">
                            <img class="w-20 h-20 object-cover rounded-full border-2 border-indigo-500" src="https://images.unsplash.com/photo-1537606845186-9921373c310f?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=334&q=80">
                        </div>
                        <div>
                            <h2 class="text-gray-800 text-3xl font-semibold">Activerend</h2>
                        </div>
                        <div class="flex justify-end mt-4">

                        </div>
                    </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="py-12 bg-blackblack">
            <div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="lg:text-center" id="onsteam">
                    <h3 class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-white sm:text-4xl sm:leading-10">
                        Creative Sessie
                    </h3>
                    <br>
                    <br>
                    <img src="/images/creative.png"/>
                    <br>

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
