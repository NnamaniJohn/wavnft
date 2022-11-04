<script setup>
import { Head } from '@inertiajs/inertia-vue3';

/* import the fontawesome core */
import { library } from '@fortawesome/fontawesome-svg-core'

/* import font awesome icon component */
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

/* import specific icons */
import { faSearch, faHouse, faClockRotateLeft } from '@fortawesome/free-solid-svg-icons'

// import { reactive } from 'vue'

/* add icons to the library */
library.add(faSearch, faHouse, faClockRotateLeft)

// const moralis = reactive({
//     serverUrl: import.meta.env.MORALIS_SERVER,
//     appId: import.meta.env.MORALIS_APP_ID
// })
//

// const serverUrl = "https://1lpkmnc4upsq.usemoralis.com:2053/server"
// const appId = "xHYtBIVG29zSwOKh5WVGcNHZl9ZoCWVCty3E3Fav"

// Moralis.start({
//     serverUrl,
//     appId
//     });

// async function login() {
//     let user = Moralis.User.current();
//     if (!user) {
//         user = await Moralis.authenticate({
//             signingMessage: "Log in using Moralis",
//         })
//             .then(function (user) {
//                 console.log("logged in user:", user);
//                 console.log(user.get("ethAddress"));
//             })
//             .catch(function (error) {
//                 console.log(error);
//             });
//     }
// }
//
// async function logOut() {
//     await Moralis.User.logOut();
//     console.log("logged out");
// }

</script>

<template>
    <Head title="WavNFTs" />

    <div class="flex flex-col h-screen">
        <header class="flex flex-row pt-5">
            <div class="w-20 text-center">
                <img src="images/icon.gif" class="w-5 h-5 mx-auto" />
                <span class="text-xs font-black">WavNFTs</span>
            </div>
            <div class="w-80 ml-3 mr-3">
                <div class="relative">
                    <input class="bg-gray-100 p-1 rounded-r-full rounded-l-full pl-8 focus:outline-none" placeholder="Search" />
                    <font-awesome-icon icon="fa-solid fa-search" class="text-gray-600 absolute bottom-2 left-2" />
                </div>
            </div>
            <div class="basis-8/12 mt-1">
                <a href="#" class="px-3 py-2 text-gray-100 rounded-l-full rounded-r-full bg-gray-600 mr-5" >Collections</a>
                <a href="#" class="px-3 py-2 text-gray-800 rounded-l-full rounded-r-full bg-gray-100 mr-5">Collections</a>
                <a href="#" class="px-3 py-2 text-gray-800 rounded-l-full rounded-r-full bg-gray-100 mr-5">Collections</a>
                <a href="#" class="px-3 py-2 text-gray-800 rounded-l-full rounded-r-full bg-gray-100 mr-5">Collections</a>
                <a href="#" class="px-3 py-2 text-gray-800 rounded-l-full rounded-r-full bg-gray-100 mr-5">Collections</a>
            </div>
        </header>

        <div class="flex flex-row w-full h-full overflow-hidden pt-2">
            <aside class="w-20 flex flex-col gap-2 justify-center text-sm text-center">
                <a class="text-gray-700 bg-gray-100 p-3 border-l-4 border-gray-700" href="#"><font-awesome-icon icon="fa-solid fa-house" /></a>
                <a class="text-gray-300 p-3 hover:bg-gray-100 hover:text-gray-700 hover:border-l-4 hover:border-gray-700" href="#"><font-awesome-icon icon="fa-solid fa-house" /></a>
                <a class="text-gray-300 p-3 hover:bg-gray-100 hover:text-gray-700 hover:border-l-4 hover:border-gray-700" href="#"><font-awesome-icon icon="fa-solid fa-house" /></a>
                <a class="text-gray-300 p-3 hover:bg-gray-100 hover:text-gray-700 hover:border-l-4 hover:border-gray-700" href="#"><font-awesome-icon icon="fa-solid fa-house" /></a>
                <a class="text-gray-300 p-3 hover:bg-gray-100 hover:text-gray-700 hover:border-l-4 hover:border-gray-700" href="#"><font-awesome-icon icon="fa-solid fa-house" /></a>
            </aside>
            <main class="flex flex-row w-full bg-gray-200 rounded-tl-3xl rounded-bl-3xl pl-8">
                <div class="w-1/3 pr-10 pt-8">
                    <h2 class="text-2xl font-bold ">Top NFT</h2>
                    <div class="px-5 py-10">
                        <div class="flex flex-row justify-between px-5">
                            <div class="flex flex-col">
                                <span class="text-gray-400 text-xs">Rarity lvl</span>
                                <span class="text-md font-bold">9.8</span>
                            </div>
                            <div class="flex flex-col text-right">
                                <span class="text-gray-400 text-xs">NFT type</span>
                                <span class="text-xs font-bold">Legend</span>
                            </div>
                        </div>
                        <div class="w-52 p-8 mx-auto flex justify-center relative bg-gray-300 rounded-full border-2 border-gray-100">
                            <img src="images/1.jpg" class="w-10 border-1 border-gray-400 rounded-t-2xl rounded-b-3xl absolute bottom-48">
                            <img src="images/11.jpg" class="w-44 rounded-full border-2 border-gray-100 p-1">
                            <span class="absolute bottom-16 right-2 backdrop-opacity-30 backdrop-invert bg-white/30 border-2 rounded-lg text-white text-xs p-1 text-center">#336M97</span>
                            <span class="absolute bottom-0 rounded-t-2xl rounded-b-full p-1 bg-gray-50 font-bold text-xs">01</span>
                        </div>
                        <div class="text-center mt-3">
                            <span class="font-bold text-2xl">DRQ_#95859</span>
                            <div class="text-2xl text-gray-400">
                                - <span>ETH: 13.65 </span> -
                            </div>
                        </div>
                    </div>
                </div>
                <div class="w-2/3 overflow-x-auto pr-5">
                    <h3 class="text-2xl font-bold mb-5 mt-8">Rare NFT</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                        <div class="bg-blue-50 border-2 border-white rounded-3xl p-2">
                            <div class="bg-white p-2 rounded-2xl">
                                <div class="flex flex-row justify-between pb-2">
                                    <div class="flex">
                                        <img src="images/11.jpg" class="rounded-full w-8">
                                        <div class="flex flex-col ml-2">
                                            <span class="text-xs">Created by</span>
                                            <span class="text-sm font-bold">35642</span>
                                        </div>
                                    </div>
                                    <div class="flex">
                                        <div class="flex flex-col mr-2 text-right">
                                            <span class="text-xs">Owned by</span>
                                            <span class="text-sm font-bold">35642</span>
                                        </div>
                                        <img src="images/11.jpg" class="rounded-full w-8">
                                    </div>
                                </div>
                                <div class="aspect-h-6 aspect-w-9 ">
                                    <img src="images/11.jpg" class="rounded-xl">
                                </div>
                            </div>
                            <div class="text-xs text-center px-4 py-2">
                                <span class="font-bold">Price: </span> ETH 5.56- X1 = ( $74,563 )
                            </div>
                            <div class="bg-white rounded-t-lg rounded-b-3xl p-2">
                                <a href="#" class="inline-block w-1/2 rounded-lg rounded-bl-3xl text-center text-sm font-bold py-3"><font-awesome-icon icon="fa-solid fa-clock-rotate-left" /> History</a>
                                <a href="#" class="inline-block w-1/2 bg-gray-700 rounded-lg rounded-br-3xl text-center text-sm text-gray-100 font-bold py-3">Buy Now</a>
                            </div>
                        </div>
                        <div class="bg-blue-50 border-2 border-white rounded-3xl p-2">
                            <div class="bg-white p-2 rounded-2xl">
                                <div class="flex flex-row justify-between pb-2">
                                    <div class="flex">
                                        <img src="images/11.jpg" class="rounded-full w-8">
                                        <div class="flex flex-col ml-2">
                                            <span class="text-xs">Created by</span>
                                            <span class="text-sm font-bold">35642</span>
                                        </div>
                                    </div>
                                    <div class="flex">
                                        <div class="flex flex-col mr-2 text-right">
                                            <span class="text-xs">Owned by</span>
                                            <span class="text-sm font-bold">35642</span>
                                        </div>
                                        <img src="images/11.jpg" class="rounded-full w-8">
                                    </div>
                                </div>
                                <div class="aspect-h-6 aspect-w-9 ">
                                    <img src="images/11.jpg" class="rounded-xl">
                                </div>
                            </div>
                            <div class="text-xs text-center px-4 py-2">
                                <span class="font-bold">Price: </span> ETH 5.56- X1 = ($74,563)
                            </div>
                            <div class="bg-white rounded-t-lg rounded-b-3xl p-2">
                                <a href="#" class="inline-block w-1/2 rounded-lg rounded-bl-3xl text-center text-sm font-bold py-3"><font-awesome-icon icon="fa-solid fa-clock-rotate-left" /> History</a>
                                <a href="#" class="inline-block w-1/2 bg-gray-700 rounded-lg rounded-br-3xl text-center text-sm text-gray-100 font-bold py-3">Buy Now</a>
                            </div>
                        </div>
                        <div class="bg-blue-50 border-2 border-white rounded-3xl p-2">
                            <div class="bg-white p-2 rounded-2xl">
                                <div class="flex flex-row justify-between pb-2">
                                    <div class="flex">
                                        <img src="images/11.jpg" class="rounded-full w-8">
                                        <div class="flex flex-col ml-2">
                                            <span class="text-xs">Created by</span>
                                            <span class="text-sm font-bold">35642</span>
                                        </div>
                                    </div>
                                    <div class="flex">
                                        <div class="flex flex-col mr-2 text-right">
                                            <span class="text-xs">Owned by</span>
                                            <span class="text-sm font-bold">35642</span>
                                        </div>
                                        <img src="images/11.jpg" class="rounded-full w-8">
                                    </div>
                                </div>
                                <div class="aspect-h-6 aspect-w-9 ">
                                    <img src="images/11.jpg" class="rounded-xl">
                                </div>
                            </div>
                            <div class="text-xs text-center px-4 py-2">
                                <span class="font-bold">Price: </span> ETH 5.56- X1 = ($74,563)
                            </div>
                            <div class="bg-white rounded-t-lg rounded-b-3xl p-2">
                                <a href="#" class="inline-block w-1/2 rounded-lg rounded-bl-3xl text-center text-sm font-bold py-3"><font-awesome-icon icon="fa-solid fa-clock-rotate-left" /> History</a>
                                <a href="#" class="inline-block w-1/2 bg-gray-700 rounded-lg rounded-br-3xl text-center text-sm text-gray-100 font-bold py-3">Buy Now</a>
                            </div>
                        </div>
                        <div class="bg-blue-50 border-2 border-white rounded-3xl p-2">
                            <div class="bg-white p-2 rounded-2xl">
                                <div class="flex flex-row justify-between pb-2">
                                    <div class="flex">
                                        <img src="images/11.jpg" class="rounded-full w-8">
                                        <div class="flex flex-col ml-2">
                                            <span class="text-xs">Created by</span>
                                            <span class="text-sm font-bold">35642</span>
                                        </div>
                                    </div>
                                    <div class="flex">
                                        <div class="flex flex-col mr-2 text-right">
                                            <span class="text-xs">Owned by</span>
                                            <span class="text-sm font-bold">35642</span>
                                        </div>
                                        <img src="images/11.jpg" class="rounded-full w-8">
                                    </div>
                                </div>
                                <div class="aspect-h-6 aspect-w-9 ">
                                    <img src="images/11.jpg" class="rounded-xl">
                                </div>
                            </div>
                            <div class="text-xs text-center px-4 py-2">
                                <span class="font-bold">Price: </span> ETH 5.56- X1 = ($74,563)
                            </div>
                            <div class="bg-white rounded-t-lg rounded-b-3xl p-2">
                                <a href="#" class="inline-block w-1/2 rounded-lg rounded-bl-3xl text-center text-sm font-bold py-3"><font-awesome-icon icon="fa-solid fa-clock-rotate-left" /> History</a>
                                <a href="#" class="inline-block w-1/2 bg-gray-700 rounded-lg rounded-br-3xl text-center text-sm text-gray-100 font-bold py-3">Buy Now</a>
                            </div>
                        </div>
                        <div class="bg-blue-50 border-2 border-white rounded-3xl p-2">
                            <div class="bg-white p-2 rounded-2xl">
                                <div class="flex flex-row justify-between pb-2">
                                    <div class="flex">
                                        <img src="images/11.jpg" class="rounded-full w-8">
                                        <div class="flex flex-col ml-2">
                                            <span class="text-xs">Created by</span>
                                            <span class="text-sm font-bold">35642</span>
                                        </div>
                                    </div>
                                    <div class="flex">
                                        <div class="flex flex-col mr-2 text-right">
                                            <span class="text-xs">Owned by</span>
                                            <span class="text-sm font-bold">35642</span>
                                        </div>
                                        <img src="images/11.jpg" class="rounded-full w-8">
                                    </div>
                                </div>
                                <div class="aspect-h-6 aspect-w-9 ">
                                    <img src="images/11.jpg" class="rounded-xl">
                                </div>
                            </div>
                            <div class="text-xs text-center px-4 py-2">
                                <span class="font-bold">Price: </span> ETH 5.56- X1 = ($74,563)
                            </div>
                            <div class="bg-white rounded-t-lg rounded-b-3xl p-2">
                                <a href="#" class="inline-block w-1/2 rounded-lg rounded-bl-3xl text-center text-sm font-bold py-3"><font-awesome-icon icon="fa-solid fa-clock-rotate-left" /> History</a>
                                <a href="#" class="inline-block w-1/2 bg-gray-700 rounded-lg rounded-br-3xl text-center text-sm text-gray-100 font-bold py-3">Buy Now</a>
                            </div>
                        </div>
                        <div class="bg-blue-50 border-2 border-white rounded-3xl p-2">
                        <div class="bg-white p-2 rounded-2xl">
                            <div class="flex flex-row justify-between pb-2">
                                <div class="flex">
                                    <img src="images/11.jpg" class="rounded-full w-8">
                                    <div class="flex flex-col ml-2">
                                        <span class="text-xs">Created by</span>
                                        <span class="text-sm font-bold">35642</span>
                                    </div>
                                </div>
                                <div class="flex">
                                    <div class="flex flex-col mr-2 text-right">
                                        <span class="text-xs">Owned by</span>
                                        <span class="text-sm font-bold">35642</span>
                                    </div>
                                    <img src="images/11.jpg" class="rounded-full w-8">
                                </div>
                            </div>
                            <div class="aspect-h-6 aspect-w-9 ">
                                <img src="images/11.jpg" class="rounded-xl">
                            </div>
                        </div>
                        <div class="text-xs text-center px-4 py-2">
                            <span class="font-bold">Price: </span> ETH 5.56- X1 = ($74,563)
                        </div>
                        <div class="bg-white rounded-t-lg rounded-b-3xl p-2">
                            <a href="#" class="inline-block w-1/2 rounded-lg rounded-bl-3xl text-center text-sm font-bold py-3"><font-awesome-icon icon="fa-solid fa-clock-rotate-left" /> History</a>
                            <a href="#" class="inline-block w-1/2 bg-gray-700 rounded-lg rounded-br-3xl text-center text-sm text-gray-100 font-bold py-3">Buy Now</a>
                        </div>
                    </div>
                        <div class="bg-blue-50 border-2 border-white rounded-3xl p-2">
                            <div class="bg-white p-2 rounded-2xl">
                                <div class="flex flex-row justify-between pb-2">
                                    <div class="flex">
                                        <img src="images/11.jpg" class="rounded-full w-8">
                                        <div class="flex flex-col ml-2">
                                            <span class="text-xs">Created by</span>
                                            <span class="text-sm font-bold">35642</span>
                                        </div>
                                    </div>
                                    <div class="flex">
                                        <div class="flex flex-col mr-2 text-right">
                                            <span class="text-xs">Owned by</span>
                                            <span class="text-sm font-bold">35642</span>
                                        </div>
                                        <img src="images/11.jpg" class="rounded-full w-8">
                                    </div>
                                </div>
                                <div class="aspect-h-6 aspect-w-9 ">
                                    <img src="images/11.jpg" class="rounded-xl">
                                </div>
                            </div>
                            <div class="text-xs text-center px-4 py-2">
                                <span class="font-bold">Price: </span> ETH 5.56- X1 = ($74,563)
                            </div>
                            <div class="bg-white rounded-t-lg rounded-b-3xl p-2">
                                <a href="#" class="inline-block w-1/2 rounded-lg rounded-bl-3xl text-center text-sm font-bold py-3"><font-awesome-icon icon="fa-solid fa-clock-rotate-left" /> History</a>
                                <a href="#" class="inline-block w-1/2 bg-gray-700 rounded-lg rounded-br-3xl text-center text-sm text-gray-100 font-bold py-3">Buy Now</a>
                            </div>
                        </div>
                    </div>
                </div>
            </main>
        </div>

        <footer class="h-20 flex flex-row justify-between items-center">
            <div class="ml-20">
                <a href="#" class="mr-3">Filter</a>
                <a href="#">Popular</a>
            </div>
            <div class="w-20">
                <span>5/100</span>
            </div>
        </footer>
    </div>

</template>
