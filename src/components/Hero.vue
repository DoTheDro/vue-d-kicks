<script>
    export default {
        data() {
            return {
                heroImage: '/src/assets/images/image-shoe.png'
            }
        }
    }
</script>

<template>
    <div class="px-3 custom-height custom-bg-color">
        <div >
            <img class="image-flip" :src="heroImage" alt="Hero Section Image">
        </div>

        <div class="-mt-10 flex flex-col gap-4">
            <h1 class="text-4xl text-gray-100 font-bold">Lorem, ipsum dolor.</h1>
            <p class="text-lg text-gray-100">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis, ipsam?</p>
        </div>
    </div>
</template>