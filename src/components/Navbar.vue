<script>
    export default {
        data() {
            return {
                siteLogo: 'src/assets/images/logo-image.png'
            }
        }
    }
</script>

<template>
    <header>
        <div class="bg-gray-800 pb-4 mb-5 box-shadow">
            <div class="w-full pb-5">
                <a class="p-2 w-2/5 flex m-auto border-white border-2 rounded-full" href="/">
                    <img class="rounded-full" :src="siteLogo" alt="Site Logo Img">
                </a>
            </div>
            <div>
                <ul class="flex justify-evenly">
                    <li class="text-gray-100 text-xl">
                        <a href="#">About Us</a>
                    </li>
                    
                    <li class="text-gray-100 text-xl">
                        <a href="#">Shop</a>
                    </li>
                    
                    <li class="text-gray-100 text-xl">
                        <a href="#">Reservations</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>