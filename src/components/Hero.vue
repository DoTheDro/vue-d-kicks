<script>
    import heroImage from '../assets/images/image-shoe.png'

    export default {
        data() {
            return {
                heroImage: heroImage
            }
        }
    }
</script>

<template>
    <div class="px-3 custom-height custom-bg-color sm:flex sm:items-center sm:flex-row-reverse md:max-w-7xl md:m-auto">
        <div class="sm:w-6/12 sm:inline-block md:w-3/5">
            <img class="image-flip" :src="heroImage" alt="Hero Section Image">
        </div>

        <div class="-mt-10 flex flex-col gap-4 sm:w-6/12 sm:m-0 sm:inline-block md:w-2/5">
            <h1 class="text-4xl text-gray-100 font-bold">Lorem, ipsum dolor.</h1>
            <p class="text-lg text-gray-100">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis, ipsam?</p>
        </div>
    </div>
</template>