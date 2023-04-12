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
    <div class="px-3 flex flex-col gap-5 mb-28">
        <h2 class="text-3xl text-gray-100 font-bold text-center underline">
            About Us
        </h2>
        <div class="flex flex-col gap-6">
            <div>
                <img :src="image" alt="About Us Image">
            </div>

            <div>
                <p class="text-lg text-gray-100 text-center">Lorem ipsum dolor sit, amet consectetur adipisicing elit. A earum, ex ut placeat quos eveniet fuga! Obcaecati debitis consequuntur consequatur molestiae quis natus ipsa dolorem illo voluptatem sint! Cumque magnam commodi voluptate, quos libero ea laudantium iste unde, consequatur, quas eum culpa. Veniam officia quisquam qui nisi possimus ipsum quae!</p>
            </div>
        </div>
    </div>
</template>