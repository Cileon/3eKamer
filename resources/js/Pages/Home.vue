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
                                                class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-700 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-700 transition duration-150 ease-in-out"
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
                                <a class="font-medium text-gray-700 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out"
                                   href="#">Home</a>
                                <a class="ml-8 font-medium text-gray-700 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out"
                                   href="#">About</a>
                                <a class="ml-8 font-medium text-gray-700 hover:text-gray-900 focus:outline-none focus:text-gray-900 transition duration-150 ease-in-out"
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
                                                class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-700 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-700 transition duration-150 ease-in-out"
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
                            <p class="mt-3 text-base text-gray-700 sm:mt-5 sm:text-lg sm:max-w-xl sm:mx-auto md:mt-5 md:text-xl lg:mx-0">
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
                        De situatie</p>
                    <h3 class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl sm:leading-10">
                        Onze visie
                    </h3>
                    <p class="mt-4 max-w-4xl text-xl leading-7 text-gray-700 lg:mx-auto">
                        Vele jongeren zijn nog niet op de hoogte van het chillingseffect. De privacy regels worden met de dag overtreden, maar ook weer aangescherpt. 
						DING is een online platform waar je kan discussieren over deze onderwerpen en dat in anonieme virtuele omgeving. Vele jongeren weten nog niet wat 
						de impact van privacy breuken kunnen zijn over een langere termijn. Met DING kunnen we deze onderwerpen bespreekbaar maken en met andere jongvolwassenen 
						het hier over hebben. Je kan zien of je op één lijn staat met elkaar, of er juist andere ideeen en meningen zijn over privacy gevoelige onderwerpen.
                    </p>
                </div>
                <div class="lg:text-center">
                    <p class="text-base leading-6 text-indigo-600 font-semibold tracking-wide uppercase mt-12">
                        Online Debat</p>
                    <h3 class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl sm:leading-10">
                        Een betere manier om sociale vraagstukken voor te leggen
                    </h3>
                    <p class="mt-4 max-w-4xl text-xl leading-7 text-gray-700 lg:mx-auto">
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
                                    <p class="mt-2 text-base leading-6 text-gray-700">
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
                                            <path d="M13 10V3L4 14h7v7l9-11h-7z" stroke-linecap="round"
                                                  stroke-linejoin="round"
                                                  stroke-width="2"/>
                                        </svg>
                                    </div>
                                </div>
                                <div class="ml-4">
                                    <h5 class="text-lg leading-6 font-medium text-gray-900">Anonimiteit</h5>
                                    <p class="mt-2 text-base leading-6 text-gray-700">
                                        DING waarborgt jouw privacy. Om deze reden kiezen we ervoor om geen data van jou op te slaan. Ook geen account of dat soort onzin. Je bent gewoon anoniem. De gebruikersnaam voor in de kamer krijg je van ons.
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
                                        technologie</h5>
                                    <p class="mt-2 text-base leading-6 text-gray-700">
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
                    <p class="mt-4 max-w-2xl text-xl leading-7 text-gray-700 lg:mx-auto">
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
                    <p class="mt-4 max-w-2xl text-xl leading-7 text-gray-200 lg:mx-auto">
                        Je ziet hier vier kernvragen. Deze vragen zijn o.a. Beantwoord vanuit het Google Form formulier wat we in het begin verstuurd hebben.
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
                        <div class="bg-white shadow-lg rounded-lg p-8 mt-8">
							<p class="text-base leading-6  font-semibold tracking-wide uppercase">Onderzoekmethodes</p>
							<div class="flex flex-wrap  text-center text-2xl my-2">
								<div class="w-1/2 my-2">
									Deskresearch.
								</div>
								<div class="w-1/2 my-2">
									Online enquete.
								</div>
								<p class="mt-4 max-w-2xl text-xl leading-7  lg:mx-auto">
									86% is niet bewust va het Chillings effect
									80% is geïnteresseerd in meer te weten te komen over hun data gebruik. Hier wilt men over spreken.

									Om over het Chillings effect te kunnen spreken zullen verschillende DING-kamers als onderwerp Chilling Effect hebben. 
									Hierin kan relevante informatie besproken worden met de mensen die op dat moment deelnemen aan het debat.
								</p>
							</div>
                    	</div>
						<div class="bg-white shadow-lg rounded-lg p-8 mt-8">
							<p class="text-base leading-6  font-semibold tracking-wide uppercase">Bronnenlijst</p>
							<div class="flex flex-wrap my-1">
								<p class="mt-4 text-m text-left lg:mx-auto">
									www.headspace.com/blog/2017/05/21/nice-irl-mean-online/ <br>
									www.theguardian.com/media-network/2015/sep/24/online-offline-personality-digital-identity <br>
									www.frankwatching.com/archive/2015/05/28/jongeren-vinden-communicatie-in-real-life-stressvol-onderzoek/ <br>
									www.policyreview.info/articles/analysis/internet-surveillance-regulation-and-chilling-effects-online-comparative-case<br>
									Griffith, R. (1978). The Chilling Effect. The Wilson Quarterly (1976-), 2(3), 135-137. Retrieved March 3, 2020, from www.jstor.org/stable/40255463 <br>
									Project-F. `Tegenwoordig speelt social media een grote rol in mijn leven. Ik ben bereid om te kopen via Facebook.` Pinar Arslan (Student) <br>
								</p>
							</div>
                    	</div>
                </div>
   <div class="text-center text-xl text-white mt-24 italic">"Veel jongeren willen de controle over hun persoonsgegevens dus wel in eigen handen nemen om
       baas te blijven over hun online imago, maar zijn op institutioneel niveau, bijv. in het controleren of
       voorkomen van de ‘schimmige’ kanten van datamining, minder daadkrachtig."</div>

            </div>
            <h3 class="mt-8 text-3xl leading-8 font-extrabold text-center tracking-tight text-white sm:text-4xl sm:leading-10">
                Empathie
            </h3>
            <p class="mt-4 max-w-2xl text-xl leading-7 text-white  lg:mx-auto">
            Anoniem je mening geven en hierover discussieren met andere. Wij begrijpen dat dit iets is waar veel jongeren naar verlangen, wij doen dit namelijk zelf ook. Uit ons onderzoek is gebleken dat niet iedereen zich volledig anoniem voelt via praat medium dus willen wij de ultieme anonieme ervaring bieden voor de gebruikers. Een virtuele omgeving waar zij zonder een identitieit hun gedachtes los kunnen laten gaan en hun rauwe mening kunnen geven.
            </p>

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
                            Uit ons onderzoek is gebleken dat jongeren die bewust of onbewust bezig zijn met privacy, wel bereid zijn om meer te willen weten over totale privacy. Of hier een eventuele discussie over te houden. 
							Ze willen graag een plek waar zij hun mening en vragen kwijt kunnen zonder raar aangekeken te worden.
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
                            Het ontwerp moet impact creëren zodat het niet alleen een goed concept is maar daadwerkelijk kan leiden tot een veiligere omgeving voor ons allemaal.
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
                            Het ontwerp moet bewustwoording creëren omdat uit ons onderzoek blijkt dat 86% van de jongeren niet bewust is van de privacy risico's op platformen zoals Instagram, Twitter en Facebook.
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
                            Het ontwerp moet jongeren stimuleren om zelf tot actie te komen. Uit ons onderzoek is gebleken dat vijftien procent wel bewust is van eventuele privacy risico's, 
							maar niet veel doen als het gaat om deze privacy veiligheid te waarborgen. 
                        </div>
                    </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="py-12 bg-blackblack">
            <div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
                <div id="onsteam">
                    <h3 class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-white sm:text-4xl sm:leading-10 mb-4 text-center">
                        Creative Sessie
                    </h3>
                    <img src="/images/creative.png"/>
                    <br>
                    <div class="flex flex-wrap text-white text-2xl my-2">
                        <div class="w-full my-2">
							<p class="mt-4 max-w-2xl text-xl leading-7 lg:mx-auto">
								Op dit blad zie je alle mogelijke ideeën die we hadden bedacht voor dit project. 
								Deze brainstorm is gehouden in een van de eerste weken van de design challenge. Over deze brainstorm sessie zijn uiteindelijk een aantal concepten gekomen.</p>
                        </div>
                        
                    </div>
                    <div class="bg-white shadow-lg rounded-lg p-8 mt-8">
                    <h3 class="mt-8 text-3xl leading-8 font-extrabold tracking-tight sm:text-4xl sm:leading-10 mb-4 text-center">
                       Idee vorming
                    </h3>
                    <div class="mt-4 max-w-2xl text-xl leading-7 lg:mx-auto">
						Tijdens onze brainstormsessies zijn we met verschillende ideeën gekomen. We hebben deze ideeën gecreëerd door gebruik te maken van een how might we methode en de braindump methode. 
						Door deze twee methodes toe te passen en te discussiëren over onze uitkomsten zijn we uitgekomen op drie ideeën.</div>
						<div class="mt-10"></div>
						<p class="mt-4 max-w-2xl text-xl leading-7 lg:mx-auto">
						Deze drie ideeën zijn Sitemap of Data, Privacy Game en de 3e kamer. De derde kamer hebben we omgedoopt tot DING waar je in de onepager verder over kan lezen. Sitemap of Data was een idee 
						om op een openbare plek een scherm neer te zetten en mensen te interviewen. Met deze informatie kunnen we online openbare data opzoeken van deze persoon en een profiel op het scherm laten zien. 
						Zo kunnen we de persoon bewust maken van de data die hij/zij achterlaat op het internet. Privacy game was een idee om een soort van price is right te maken. Maar daar kom je aan zet door middel van 
						het vrijgeven van je data.</p>
						<div class="mt-10"></div>
						<p class="mt-4 max-w-2xl text-xl leading-7 lg:mx-auto">
						We hebben de ideeën gekozen door onze ontwerprichtlijnen centraal te houden, daardoor sluiten al deze ideeën aan op onze ontwerpkeuzes. Sitemap of Data en Privacy Game zijn voor ons afgevallen door 
						de corona-crisis, aangezien we DING (de derde kamer) het best in een online omgeving kunnen realiseren. Dit is de beste keuze omdat voor de andere twee ideeën wij persoonlijk aanwezig moeten zijn om dit 
						in een goede baan te kunnen leiden; Sitemap, iemand moet de persoon interviewen en een anders zijn data opzoeken en in een diagram zetten. Privacy Game, we hebben een host nodig publiek en productie. Voor 
						DING kunnen we een veelal autonoom project opzetten. Deze applicatie kan werken zonder dat wij daar invloed op hebben. Bij DING hadden we eerst ook een idee om hiervan een installatie te maken. Door een tent 
						op te zetten en hierin te discussiëren, met sprekers en publiek. Maar door corona hebben we dit omgezet naar een online omgeving waar toevallig ook een goed gevolg aan zit. De online omgeving die we willen 
						creëren geeft meer privacy en meer animo voor onze doelgroep ten opzichte van een discussie op locatie.</p>
						<div class="mt-10"></div>
						<p class="mt-4 max-w-2xl text-xl leading-7 lg:mx-auto">
						DING heeft voor ons de juiste bedoelingen maar kan ook veel breder ingezet worden voor andere maatschappelijke problemen. Wij kunnen hier inspelen op veel verschillende meningen en deze ook laten 
						horen door bij andere bewustwording te creëren.</p>
					</div>
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
