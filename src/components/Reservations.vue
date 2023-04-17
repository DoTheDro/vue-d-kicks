<script>
    import imageFloat from '../assets/images/image-bg.png'

    export default {
        data() {
            return {
                text: 'Sample text reservations',
                image: imageFloat
            }
        }
    }
</script>

<template>
    <div data-aos="zoom-in-up"
        data-aos-duration="700"
        data-aos-once="true"
    class="px-3 py-4 flex flex-col gap-5 mb-28 relative height-cust" id="reservations">
        <img class="absolute left-0 height-cust top-1 z-0" :src="image" alt="image background">
        <div class="bg-gray-950 bg-opacity-60 height-cust flex flex-col justify-around px-3 py-4 z-10 rounded-lg sm:justify-center sm:gap-8 sm:max-w-2xl sm:m-auto">
            <h2 class="text-3xl text-gray-100 font-bold text-center underline">Reservations</h2>
            <p class="text-lg text-gray-100 text-center">Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora numquam mollitia, quam blanditiis sunt consequuntur temporibus nesciunt, nobis optio, eaque provident reprehenderit! Odit odio, iure tempora rem similique officiis impedit exercitationem suscipit ipsam natus nostrum autem? Itaque, consequatur, tenetur ab quod magni totam nisi ratione omnis, quo voluptatibus soluta repellat.</p>
        </div>
    </div>
</template>