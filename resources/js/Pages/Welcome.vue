<script setup>
import { Head, Link } from '@inertiajs/inertia-vue3';

/* import the fontawesome core */
import { library } from '@fortawesome/fontawesome-svg-core'

/* import font awesome icon component */
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';

import {faSearch, faLocationDot, faTag, faHouse, faBars, faCircleArrowDown} from '@fortawesome/free-solid-svg-icons';

library.add(faSearch, faLocationDot, faTag, faHouse, faBars, faCircleArrowDown)

</script>

<template>
    <Head title="Welcome" />

    <header class="bg-[url('images/houses/d08.png')] bg-cover bg-center h-screen pb-32">
        <div class="container">
            <nav class="flex items-center">
                <div>
                    <svg class="w-24 h-16" xmlns="http://www.w3.org/2000/svg" width="1427.731" height="472.472" viewBox="0 0 1427.731 472.472">
                        <g id="Path_1" data-name="Path 1" transform="matrix(0.927, -0.375, 0.375, 0.927, 0, 164.18)" fill="#f11b1b">
                            <path d="M 0.8615646958351135 168.6633605957031 L 94.52164459228516 1.042917728424072 L 182.1295471191406 165.1329040527344 L 0.8615646958351135 168.6633605957031 Z" stroke="none"/>
                            <path d="M 94.51166534423828 2.085845947265625 L 1.723159790039062 168.146484375 L 181.3043365478516 164.6489105224609 L 94.51166534423828 2.085845947265625 M 94.53162384033203 0 L 182.9547729492188 165.6169586181641 L 0 169.1802368164062 L 94.53162384033203 0 Z" stroke="none" fill="#707070"/>
                        </g>
                        <g id="Path_2" data-name="Path 2" transform="matrix(0.927, -0.375, 0.375, 0.927, 61.549, 137.121)" fill="#f8f8f8">
                            <path d="M -5.827252388000488 170.9443359375 L 90.15986633300781 -2.763704061508179 L 176.2940216064453 165.2455139160156 L -5.827252388000488 170.9443359375 Z" stroke="none"/>
                            <path d="M 90.143310546875 -1.699966430664062 L -4.964691162109375 170.4170989990234 L 175.4885864257812 164.7704772949219 L 90.143310546875 -1.699966430664062 M 90.17638397216797 -3.827438354492188 L 177.0994262695312 165.7205505371094 L -6.68988037109375 171.4715728759766 L 90.17638397216797 -3.827438354492188 Z" stroke="none" fill="#707070"/>
                        </g>
                        <g id="Path_3" data-name="Path 3" transform="matrix(0.927, -0.375, 0.375, 0.927, 115.68, 104.559)" fill="#f11b1b">
                            <path d="M -5.9871506690979 180.6850891113281 L 93.93904876708984 -2.75898289680481 L 177.6348419189453 171.3662567138672 L -5.9871506690979 180.6850891113281 Z" stroke="none"/>
                            <path d="M 93.91123199462891 -1.662673950195312 L -5.121139526367188 180.1405029296875 L 176.8583526611328 170.9049987792969 L 93.91123199462891 -1.662673950195312 M 93.96684265136719 -3.855270385742188 L 178.4112701416016 171.8274688720703 L -6.853179931640625 181.2296905517578 L 93.96684265136719 -3.855270385742188 Z" stroke="none" fill="#707070"/>
                        </g>
                        <g id="Path_4" data-name="Path 4" transform="matrix(0.927, -0.375, 0.375, 0.927, 165.761, 87.511)" fill="#f8f8f8">
                            <path d="M -5.962715625762939 178.5571746826172 L 93.24443054199219 -2.77263617515564 L 177.4237823486328 169.9230194091797 L -5.962715625762939 178.5571746826172 Z" stroke="none"/>
                            <path d="M 93.21881103515625 -1.684051513671875 L -5.09661865234375 178.0158386230469 L 176.6414947509766 169.4593048095703 L 93.21881103515625 -1.684051513671875 M 93.27005767822266 -3.861190795898438 L 178.2060546875 170.3867492675781 L -6.828842163085938 179.0985107421875 L 93.27005767822266 -3.861190795898438 Z" stroke="none" fill="#707070"/>
                        </g>
                        <g id="Path_5" data-name="Path 5" transform="matrix(0.927, -0.375, 0.375, 0.927, 223.252, 68.536)" fill="#f11b1b">
                            <path d="M 0.8615646958351135 168.6633605957031 L 94.52164459228516 1.042917728424072 L 182.1295471191406 165.1329040527344 L 0.8615646958351135 168.6633605957031 Z" stroke="none"/>
                            <path d="M 94.51166534423828 2.085845947265625 L 1.723159790039062 168.146484375 L 181.3043365478516 164.6489105224609 L 94.51166534423828 2.085845947265625 M 94.53162384033203 0 L 182.9547729492188 165.6169586181641 L 0 169.1802368164062 L 94.53162384033203 0 Z" stroke="none" fill="#707070"/>
                        </g>
                        <g id="Path_6" data-name="Path 6" transform="matrix(-0.927, 0.375, -0.375, -0.927, 513.117, 307.382)" fill="#f11b1b">
                            <path d="M 0.8615646958351135 168.6633605957031 L 94.52164459228516 1.042917728424072 L 182.1295471191406 165.1329040527344 L 0.8615646958351135 168.6633605957031 Z" stroke="none"/>
                            <path d="M 94.51166534423828 2.085845947265625 L 1.723159790039062 168.146484375 L 181.3043365478516 164.6489105224609 L 94.51166534423828 2.085845947265625 M 94.53162384033203 0 L 182.9547729492188 165.6169586181641 L 0 169.1802368164062 L 94.53162384033203 0 Z" stroke="none" fill="#707070"/>
                        </g>
                        <g id="Path_7" data-name="Path 7" transform="matrix(-0.927, 0.375, -0.375, -0.927, 449.569, 334.441)" fill="#f8f8f8">
                            <path d="M -5.827252388000488 170.9443359375 L 90.15986633300781 -2.763704061508179 L 176.2940216064453 165.2455139160156 L -5.827252388000488 170.9443359375 Z" stroke="none"/>
                            <path d="M 90.143310546875 -1.699966430664062 L -4.964691162109375 170.4170989990234 L 175.4885864257812 164.7704772949219 L 90.143310546875 -1.699966430664062 M 90.17638397216797 -3.827438354492188 L 177.0994262695312 165.7205505371094 L -6.68988037109375 171.4715728759766 L 90.17638397216797 -3.827438354492188 Z" stroke="none" fill="#707070"/>
                        </g>
                        <g id="Path_8" data-name="Path 8" transform="matrix(-0.927, 0.375, -0.375, -0.927, 399.438, 367.004)" fill="#f11b1b">
                            <path d="M -5.9871506690979 180.6850891113281 L 93.93904876708984 -2.75898289680481 L 177.6348419189453 171.3662567138672 L -5.9871506690979 180.6850891113281 Z" stroke="none"/>
                            <path d="M 93.91123199462891 -1.662673950195312 L -5.121139526367188 180.1405029296875 L 176.8583526611328 170.9049987792969 L 93.91123199462891 -1.662673950195312 M 93.96684265136719 -3.855270385742188 L 178.4112701416016 171.8274688720703 L -6.853179931640625 181.2296905517578 L 93.96684265136719 -3.855270385742188 Z" stroke="none" fill="#707070"/>
                        </g>
                        <g id="Path_9" data-name="Path 9" transform="matrix(-0.927, 0.375, -0.375, -0.927, 348.357, 384.051)" fill="#f8f8f8">
                            <path d="M -5.962715625762939 178.5571746826172 L 93.24443054199219 -2.77263617515564 L 177.4237823486328 169.9230194091797 L -5.962715625762939 178.5571746826172 Z" stroke="none"/>
                            <path d="M 93.21881103515625 -1.684051513671875 L -5.09661865234375 178.0158386230469 L 176.6414947509766 169.4593048095703 L 93.21881103515625 -1.684051513671875 M 93.27005767822266 -3.861190795898438 L 178.2060546875 170.3867492675781 L -6.828842163085938 179.0985107421875 L 93.27005767822266 -3.861190795898438 Z" stroke="none" fill="#707070"/>
                        </g>
                        <g id="Path_10" data-name="Path 10" transform="translate(293.618 400.986) rotate(157)" fill="#f11b1b">
                            <path d="M 0.8615646958351135 168.6633605957031 L 94.52164459228516 1.042917728424072 L 182.1295471191406 165.1329040527344 L 0.8615646958351135 168.6633605957031 Z" stroke="none"/>
                            <path d="M 94.51166534423828 2.085845947265625 L 1.723159790039062 168.146484375 L 181.3043365478516 164.6489105224609 L 94.51166534423828 2.085845947265625 M 94.53162384033203 0 L 182.9547729492188 165.6169586181641 L 0 169.1802368164062 L 94.53162384033203 0 Z" stroke="none" fill="#707070"/>
                        </g>
                        <text id="WAAVA" transform="translate(489.731 305.837)" fill="#fff" font-size="222" font-family="Verdana-Bold, Verdana" font-weight="700"><tspan x="0" y="0">WAAVA</tspan></text>
                    </svg>
                </div>
                <ul class="hidden sm:flex flex-1 justify-center items-center sm:gap-6 md:gap-12 text-white sm:text-xs md:text-sm uppercase font-bold">
                    <li><a href="#">About</a></li>
                    <li><a href="#">Services</a></li>
                    <li><a href="#">Project</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
                <a href="#" class="hidden sm:text-xs md:text-sm sm:inline-block bg-red-500 rounded-r-full rounded-l-full px-7 py-2">Get Started</a>
                <div class="flex sm:hidden flex-1 justify-end">
                    <font-awesome-icon class="text-white text-3xl" icon="fa-solid fa-bars" />
                </div>
            </nav>
            <h1 class="text-white text-3xl lg:text-6xl text-center font-bold mt-8 lg:mt-24">The smartest way to buy a home</h1>
            <p class="text-white font-semibold text-center text-sm max-w-xl mx-auto mt-5 mb-12">Let's find your dream home with WAAVA. Partner with local real estate agent to find the home or apartment that's is right for you.</p>
            <div class="flex flex-col sm:flex-row items-center bg-gray-100 sm:rounded-l-full sm:rounded-r-full p-3 divide-y sm:divide-y-0 sm:divide-x divide-gray-400 xl:w-9/12 sm:mx-auto text-black font-bold text-sm">
                <div class="flex flex-col flex-1 w-full sm:w-32 md:w-48 px-2 py-2 sm:px-6">
                    <label>Locations <font-awesome-icon icon="fa-solid fa-location-dot" /></label>
                    <input class="bg-gray-100 outline-0 text-gray-500" placeholder="Find destinations">
                </div>
                <div class="flex flex-col flex-1 w-full sm:w-32 md:w-48 px-2 py-2 sm:px-6">
                    <label>Budget <font-awesome-icon icon="fa-solid fa-tag" /></label>
                    <input class="bg-gray-100 outline-0 text-gray-500" placeholder="Find destinations">
                </div>
                <div class="flex flex-col flex-1 w-full sm:w-32 md:w-48 px-2 py-2 sm:px-6">
                    <label>Type of home <font-awesome-icon icon="fa-solid fa-house" /></label>
                    <input class="bg-gray-100 outline-0 text-gray-500" placeholder="Find destinations">
                </div>
                <button class="bg-red-500 sm:rounded-full w-full sm:w-16 sm:h-16 py-2 text-white"><span class="sm:hidden text-lg font-bold mr-2">Search</span><font-awesome-icon icon="fa-solid fa-search" class="md:text-3xl" /></button>
            </div>
        </div>
    </header>

    <p class="text-center text-lg md:text-2xl sm:w-11/12 md:w-10/12 lg:w-8/12 mx-auto my-8 px-3 md:px-8 py-14">Explore some of the most sought after internation destinations for luxury real estate in the world. We provides unrivaled access to distinctive properties in the finest locations worldwide, offering you awide selection of art.</p>

    <div class="bg-gray-200 py-24">
        <div class="container">
            <div class="grid grid-cols-1 sm:grid-cols-2 items-center text-center sm:text-left px-8">
                <h2 class="text-5xl font-bold py-5"> Explore our Project </h2>
                <p class="text-xl py-5">We love our residential design and build projects - big and small! From full builds, major renovations or a mew lease of life to individual space and create perfect place.</p>
            </div>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 py-16 mx-5 border-b border-solid border-gray-400">
                <div class="flex flex-col p-3 border-b sm:border-b-0 border-solid border-gray-400">
                    <div class="relative my-4 bg-gray-500 w-full h-44 flex items-center justify-center">
                        <img class="transition-opacity ease-in duration-700 hover:opacity-30 absolute w-full h-full cursor-pointer" src="images/houses/i1.jpg">
                        <font-awesome-icon icon="fa-solid fa-circle-arrow-down" class="text-center text-6xl " />
                    </div>
                    <h3 class="text-3xl font-bold py-4">Faishore Duel Haven</h3>
                    <p class="text-lg text-gray-600 py-4">Manipulating the space and livingroom in each apartment.</p>
                    <span class="text-lg text-gray-600 py-4">January 18 - 2022</span>
                </div>
                <div class="flex flex-col p-3 border-b sm:border-b-0 border-solid border-gray-400">
                    <div class="relative my-4 bg-gray-500 w-full h-44 flex items-center justify-center">
                        <img class="transition-opacity ease-in duration-700 hover:opacity-30 absolute w-full h-full cursor-pointer" src="images/houses/i2.jpg">
                        <font-awesome-icon icon="fa-solid fa-circle-arrow-down" class="text-center text-6xl " />
                    </div>
                    <h3 class="text-3xl font-bold py-4">Modern Panthouse</h3>
                    <p class="text-lg text-gray-600 py-4">Custom furnishings and window furnishings to soften the space.</p>
                    <span class="text-lg text-gray-600 py-4">January 15 - 2022</span>
                </div>
                <div class="flex flex-col p-3 border-b sm:border-b-0 border-solid border-gray-400">
                    <div class="relative my-4 bg-gray-500 w-full h-44 flex items-center justify-center">
                        <img class="transition-opacity ease-in duration-700 hover:opacity-30 absolute w-full h-full cursor-pointer" src="images/houses/i3.jpg">
                        <font-awesome-icon icon="fa-solid fa-circle-arrow-down" class="text-center text-6xl " />
                    </div>
                    <h3 class="text-3xl font-bold py-4">Faishore Home Garden</h3>
                    <p class="text-lg text-gray-600 py-4">Renovating result is a light and breezy modern home garden.</p>
                    <span class="text-lg text-gray-600 py-4">January 14 - 2022</span>
                </div>
                <div class="flex flex-col p-3 border-b sm:border-b-0 border-solid border-gray-400">
                    <div class="relative my-4 bg-gray-500 w-full h-44 flex items-center justify-center">
                        <img class="transition-opacity ease-in duration-700 hover:opacity-30 absolute w-full h-full cursor-pointer" src="images/houses/i4.jpg">
                        <font-awesome-icon icon="fa-solid fa-circle-arrow-down" class="text-center text-6xl " />
                    </div>
                    <h3 class="text-3xl font-bold py-4">Hastings Apartment</h3>
                    <p class="text-lg text-gray-600 py-4">Apartment needed cosmetic changes to bring it to life.</p>
                    <span class="text-lg text-gray-600 py-4">January 10 - 2022</span>
                </div>
            </div>
        </div>
    </div>

    <div class="grid grid-cols-1 sm:grid-cols-2 gap-8 px-20 py-32">
        <img class="w-full" src="images/houses/g01.jpg">
        <div class="flex flex-1 flex-col justify-center text-center sm:text-left px-8">
            <h2 class="text-5xl font-bold py-5"> Explore our Project </h2>
            <p class="text-xl py-5">We love our residential design and build projects - big and small! From full builds, major renovations or a mew lease of life to individual space and create perfect place.</p>
        </div>
    </div>

<!--    <div class="bg-gray-100 py-32">-->
<!--        <div class="grid grid-cols-9 px-8">-->
<!--            <div class="animate-bounce">-->
<!--                <img class="w-32 h-32 rounded-full animate-pulse" src="images/houses/i1.jpg">-->
<!--            </div>-->

<!--            <img class="w-32 h-32 rounded-full translate-y-6" src="images/houses/i1.jpg">-->
<!--            <img class="w-32 h-32 rounded-full" src="images/houses/i1.jpg">-->
<!--            <img class="w-32 h-32 rounded-full translate-y-6" src="images/houses/i1.jpg">-->
<!--            <img class="w-32 h-32 rounded-full translate-y-16" src="images/houses/i1.jpg">-->
<!--            <img class="w-32 h-32 rounded-full translate-y-6" src="images/houses/i1.jpg">-->
<!--            <img class="w-32 h-32 rounded-full" src="images/houses/i1.jpg">-->
<!--            <img class="w-32 h-32 rounded-full translate-y-6" src="images/houses/i1.jpg">-->
<!--            <img class="w-32 h-32 rounded-full translate-y-16" src="images/houses/i1.jpg">-->
<!--        </div>-->
<!--        <h3 class="text-5xl font-bold text-center">Trusted by over 150+ organizations in more than 50 countries</h3>-->

<!--    </div>-->
</template>

<style scoped>

</style>
