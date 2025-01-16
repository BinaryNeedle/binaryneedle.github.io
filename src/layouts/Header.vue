<script setup>
import { ref } from 'vue';

let mobileNav = ref(false);

let toggleMobileNav = () => {
    mobileNav.value = !mobileNav.value;
}
</script>

<template>
    <!-- Navbar Start -->
    <div class="fixed w-fit top-0 right-0 h-screen text z-50">
        <header class="flex flex-col justify-center items-end h-full px-5">
            <nav class="flex flex-col items-end">
                <ul class="space-y-7 font-theme-heading font-medium items-center hidden md:flex flex-col">
                    <li class="uppercase transition duration-200 flex items-center border border-transparent  rounded-lg  hover:border-blue-500 hover:shadow-lg hover:shadow-blue-500/50 glow-effect">
                        <a href="#about" class="flex items-center p-2">
                            <svg width="40px" height="40px" viewBox="0 0 24.00 24.00" fill="none" xmlns="http://www.w3.org/2000/svg" stroke="#000000">
                                <g id="SVGRepo_iconCarrier">
                                    <path d="M3 10H16M3 14H21M3 18H16M3 6H21" stroke="#FFFFFF" stroke-width="2.4" stroke-linecap="round" stroke-linejoin="round"></path>
                                </g>
                            </svg>
                        </a>
                    </li>
                    <li class="uppercase transition duration-200 flex items-center border border-transparent  rounded-lg   hover:border-blue-500 hover:shadow-lg hover:shadow-blue-500/50 glow-effect">
                        <a href="#project" class="flex items-center p-2">
                            <svg width="40px" height="40px" viewBox="0 0 24.00 24.00" fill="none" xmlns="http://www.w3.org/2000/svg" transform="rotate(45)">
                                <g id="SVGRepo_iconCarrier">
                                    <path d="M3 12H5M19 12H21M10 12H14M6.6 19H8.4C8.96005 19 9.24008 19 9.45399 18.891C9.64215 18.7951 9.79513 18.6422 9.89101 18.454C10 18.2401 10 17.9601 10 17.4V6.6C10 6.03995 10 5.75992 9.89101 5.54601C9.79513 5.35785 9.64215 5.20487 9.45399 5.10899C9.24008 5 8.96005 5 8.4 5H6.6C6.03995 5 5.75992 5 5.54601 5.10899C5.35785 5.20487 5.20487 5.35785 5.10899 5.54601C5 5.75992 5 6.03995 5 6.6V17.4C5 17.9601 5 18.2401 5.10899 18.454C5.20487 18.6422 5.35785 18.7951 5.54601 18.891C5.75992 19 6.03995 19 6.6 19ZM15.6 16H17.4C17.9601 16 18.2401 16 18.454 15.891C18.6422 15.7951 18.7951 15.6422 18.891 15.454C19 15.2401 19 14.9601 19 14.4V9.6C19 9.03995 19 8.75992 18.891 8.54601C18.7951 8.35785 18.6422 8.20487 18.454 8.10899C18.2401 8 17.9601 8 17.4 8H15.6C15.0399 8 14.7599 8 14.546 8.10899C14.3578 8.20487 14.2049 8.35785 14.109 8.54601C14 8.75992 14 9.03995 14 9.6 ```vue
V14.4C14 14.9601 14 15.2401 14.109 15.454C14.2049 15.6422 14.3578 15.7951 14.546 15.891C14.7599 16 15.0399 16 15.6 16Z" stroke="#FFFFFF" stroke-width="1.9200000000000004" stroke-linecap="round" stroke-linejoin="round"></path>
                                </g>
                            </svg>
                        </a>
                    </li>
                    <li class="uppercase transition duration-200 flex items-center border border-transparent  rounded-lg   hover:border-blue-500 hover:shadow-lg hover:shadow-blue-500/50 glow-effect">
                        <a href="#service" class="flex items-center p-2">
                            <svg width="40px" height="40px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" transform="rotate(0)"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M3 12H21M12 8V12M6.5 12V16M17.5 12V16M10.1 8H13.9C14.4601 8 14.7401 8 14.954 7.89101C15.1422 7.79513 15.2951 7.64215 15.391 7.45399C15.5 7.24008 15.5 6.96005 15.5 6.4V4.6C15.5 4.03995 15.5 3.75992 15.391 3.54601C15.2951 3.35785 15.1422 3.20487 14.954 3.10899C14.7401 3 14.4601 3 13.9 3H10.1C9.53995 3 9.25992 3 9.04601 3.10899C8.85785 3.20487 8.70487 3.35785 8.60899 3.54601C8.5 3.75992 8.5 4.03995 8.5 4.6V6.4C8.5 6.96005 8.5 7.24008 8.60899 7.45399C8.70487 7.64215 8.85785 7.79513 9.04601 7.89101C9.25992 8 9.53995 8 10.1 8ZM15.6 21H19.4C19.9601 21 20.2401 21 20.454 20.891C20.6422 20.7951 20.7951 20.6422 20.891 20.454C21 20.2401 21 19.9601 21 19.4V17.6C21 17.0399 21 16.7599 20.891 16.546C20.7951 16.3578 20.6422 16.2049 20.454 16.109C20.2401 16 19.9601 16 19.4 16H15.6C15.0399 16 14.7599 16 14.546 16.109C14.3578 16.2049 14.2049 16.3578 14.109 16.546C14 16.7599 14 17.0399 14 17.6V19.4C14 19.9601 14 20.2401 14.109 20.454C14.2049 20.6422 14.3578 20.7951 14.546 20.891C14.7599 21 15.0399 21 15.6 21ZM4.6 21H8.4C8.96005 21 9.24008 21 9.45399 20.891C9.64215 20.7951 9.79513 20.6422 9.89101 20.454C10 20.2401 10 19.9601 10 19.4V17.6C10 17.0399 10 16.7599 9.89101 16.546C9.79513 16.3578 9.64215 16.2049 9.45399 16.109C9.24008 16 8.96005 16 8.4 16H4.6C4.03995 16 3.75992 16 3.54601 16.109C3.35785 16.2049 3.20487 16.3578 3.10899 16.546C3 16.7599 3 17.0399 3 17.6V19.4C3 19.9601 3 20.2401 3.10899 20.454C3.20487 20.6422 3.35785 20.7951 3.54601 20.891C3.75992 21 4.03995 21 4.6 21Z" stroke="#ffffff" stroke-width="1.6799999999999997" stroke-linecap="round" stroke-linejoin="round"></path> </g></svg>
                        </a>
                    </li>
                </ul>
            </nav>
        </header>

        <!-- Mobile Menu Start-->
        <div v-show="mobileNav">
            <div class="absolute px-5 py-12 block z-30 top -0 left-0 w-full h-full bg-gradient-to-b from-theme-dark-blue via-theme-dark-blue-tp to-theme-dark-blue">
                <div class="flex justify-between items-center">
                    <!-- <img src="/images/logo-bookmark-white.svg" alt="Logo"> -->
                    <button @click="toggleMobileNav()" type="button" class="focus:outline-none">
                        <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-x text-white" viewBox="0 0 16 16">
                            <path d="M4.646 4.646a.5.5 0 0 1 .708 0L8 7.293l2.646-2.647a.5.5 0 0 1 .708.708L8.707 8l2.647 2.646a.5.5 0 0 1-.708.708L8 8.707l-2.646 2.647a.5.5 0 0 1-.708-.708L7.293 8 4.646 5.354a.5.5 0 0 1 0-.708z"/>
                        </svg>
                    </button>
                </div>
                <ul class="uppercase text-white text-md tracking-widest items-center flex flex-col mt-14">
                    <li class="hover:text-theme-secondary transition duration-200 py-4 border-t border-b border-theme-grayish-blue w-full text-center">
                        <a @click="toggleMobileNav()" href="#features">Features</a>
                    </li>
                    <li class="hover:text-theme-secondary transition duration-200 py-4 border-b border-theme-grayish-blue w-full text-center">
                        <a @click="toggleMobileNav()" href="#faq">FAQ</a>
                    </li>
                    <li class="hover:text-theme-secondary transition duration-200 py-4 border-b border-theme-grayish-blue w-full text-center">
                        <a @click="toggleMobileNav()" href="#subscribe">Subscribe</a>
                    </li>
                    <li class="bg-transparent border-2  px-6 py-2 mt-6 w-full text-center cursor-pointer hover:text-theme-secondary transition duration-200">
                        <a @click="toggleMobileNav()" href="#download-section">Download</a>
                    </li>
                </ul>
                <div class="flex justify-center items-end h-52">
                    <ul class="flex space-x-8">
                        <li>
                            <svg xmlns="http://www.w3.org/2000/svg" width="26" height="26" fill="currentColor" class="bi bi-facebook text-white hover:text-theme-secondary transition duration-200 cursor-pointer" viewBox="0 0 16 16">
                                <path d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951z"/>
                            </svg>
                        </li>
                        <li>
                            <svg xmlns="http://www.w3.org/2000/svg" width="26" height="26" fill="currentColor" class="bi bi-twitter text-white hover:text-theme-secondary transition duration-200 cursor-pointer" viewBox="0 0 16 16">
                                <path d="M5.026 15c6.038 0 9.341-5.003 9.341-9.334 0-.14 0-.282-.006-.422A6.685 6.685 0 0 0 16 3.542a6.658 6.658 0 0 1-1.889.518 3.301 3.301 0 0 0 1.447-1.817 6.533 6.533 0 0 ```vue
0 1-2.087.793A3.286 3.286 0 0 0 7.875 6.03a9.325 9.325 0 0 1-6.767-3.429 3.289 3.289 0 0 0 1.018 4.382A3.323 3.323 0 0 1 .64 6.575v.045a3.288 3.288 0 0 0 2.632 3.218 3.203 3.203 0 0 1-.865.115 3.23 3.23 0 0 1-.614-.057 3.283 3.283 0 0 0 3.067 2.277A6.588 6.588 0 0 1 .78 13.58a6.32 6.32 0 0 1-.78-.045A9.344 9.344 0 0 0 5.026 15z"/>
                            </svg>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <!-- Mobile Menu End-->
    </div>
    <!-- Navbar End -->
</template>
