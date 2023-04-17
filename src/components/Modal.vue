<script>
    export default {
        props: ['content'],
        methods: {
            closeModal() {
                this.$emit('close')
            }
        }
    }
</script>

<template>
    <div data-aos="zoom-out"
        data-aos-duration="300"
    class="w-full h-screen bg-black bg-opacity-80 top-0 left-0 fixed flex items-center justify-center z-40 px-4" @click.self="closeModal">
        <div class="h-3/4 w-full bg-gray-100 flex flex-col justify-evenly rounded-lg p-4 max-w-md md:max-w-3xl md:flex-row md:h-3/5 md:items-center">
            <div class="md:w-6/12 md:inline-block md:pr-5">
                <img :src="content['image']" :alt="content['name']">
            </div>
            <div class="flex flex-col gap-2 md:w-6/12 md:inline-flex">
                <div class="flex flex-col gap-2">
                    <h2 class="text-2xl font-medium md:text-4xl">
                        {{ content['name'] }}
                    </h2>
                    <h3 class="text-xl font-medium md:text-2xl">
                        $ {{ content['price'] }}
                    </h3>
                </div>
                <div class="flex flex-col gap-2">
                    <p class="text-base text-normal md:text-lg">
                        Product description: {{ content['description'] }}
                    </p>
                    <p class="text-base text-normal md:text-lg">
                        Brand: <span class="font-bold">{{ content['brand'].charAt(0).toUpperCase() + content['brand'].slice(1) }}</span>
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>