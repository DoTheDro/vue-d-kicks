<script>
    import aboutUsImg from '../assets/images/hero-section-image.png'

    export default {
        data() {
            return {
                image: aboutUsImg
            }
        }
    }
</script>

<template>
    <div class="mx-3 px-4 py-6 flex flex-col gap-5 mb-28 bg-gray-700 rounded-lg box-shadow sm:gap-9 md:max-w-7xl md:mx-auto">
        <h2 class="text-3xl text-gray-100 font-bold text-center underline">
            About Us
        </h2>
        <div class="flex flex-col gap-6 sm:flex-row sm:items-center md:justify-center">
            <div class="sm:w-6/12 sm:inline-block md:max-w-lg">
                <img :src="image" alt="About Us Image">
            </div>

            <div class="sm:w-6/12 sm:inline-block">
                <p class="text-lg text-gray-100 text-center sm:text-left sm:text-xl">Lorem ipsum dolor sit, amet consectetur adipisicing elit. A earum, ex ut placeat quos eveniet fuga! Obcaecati debitis consequuntur consequatur molestiae quis natus ipsa dolorem illo voluptatem sint! Cumque magnam commodi voluptate, quos libero ea laudantium iste unde, consequatur, quas eum culpa. Veniam officia quisquam qui nisi possimus ipsum quae!</p>
            </div>
        </div>
    </div>
</template>