<script>
    import siteLogo from '../assets/images/logo-image.png'

    export default {
        data() {
            return {
                logo: siteLogo
            }
        }
    }
</script>

<template>
    <header>
        <div class="bg-gray-800 pb-4 mb-2 box-shadow sm:pt-4 sm:flex sm:align-center md:justify-center">
            <div class="w-full pb-5 sm:w-6/12 sm:inline-flex sm:pb-0 sm:pl-4 md:max-w-screen-sm">
                <a class="p-2 w-2/5 flex m-auto border-white border-2 rounded-full custom-max-width sm:m-0" href="/">
                    <img class="rounded-full" :src="logo" alt="Site Logo Img">
                </a>
            </div>
            <div class="sm:w-6/12 sm:inline-flex sm:justify-end sm:pr-4 sm:items-center md:max-w-screen-sm">
                <ul class="flex justify-evenly sm:gap-8">
                    <li class="text-gray-100 text-xl">
                        <a href="#about">About Us</a>
                    </li>
                    
                    <li class="text-gray-100 text-xl">
                        <a href="#shop">Shop</a>
                    </li>
                    
                    <li class="text-gray-100 text-xl">
                        <a href="#reservations">Reservations</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>