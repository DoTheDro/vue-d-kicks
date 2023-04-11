<script>
    export default {
        data() {
            return {
                products: [
                    { name: 'Adidas Sneaker', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: '/src/assets/images/adidas-shoe-sneakers.png', price: '187.00', brand: 'adidas' },
                    { name: 'Yeezy', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: '/src/assets/images/adidas-yeezy.png', price: '135.00', brand: 'adidas' },
                    { name: 'Air Max', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: '/src/assets/images/nike-air-max.png', price: '150.00', brand: 'nike' },
                    { name: 'Air Max Zoom', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: '/src/assets/images/shoe-nike-air-max.png', price: '198.00', brand: 'nike' },
                    { name: 'Nike Sneaker', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: '/src/assets/images/sneaker-nike-shoe.png', price: '186.00', brand: 'nike' },
                    { name: 'Sneaker Stan Smith', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: '/src/assets/images/sneakers-adidas-stan-smith.png', price: '108.00', brand: 'adidas' },
                    { name: 'Sneaker', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: '/src/assets/images/sneakers-basketball.png', price: '200.00', brand: 'nike' },
                    { name: 'Adidas Skater', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: '/src/assets/images/sneakers-skate-shoe.png', price: '107.00', brand: 'adidas' },
                    { name: 'Old Skool', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: '/src/assets/images/vans-old-skool.png', price: '101.00', brand: 'vans' },
                    { name: 'Skater - Fire', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: '/src/assets/images/vans-skate-shoe-fire.png', price: '192.00', brand: 'vans' },
                    { name: 'Vans Skater', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: '/src/assets/images/vans-skate-shoe.png', price: '147.00', brand: 'vans' },
                    { name: 'Vans Slip-on', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: '/src/assets/images/vans-slip-on-shoe.png', price: '108.00', brand: 'vans' },
                ]
            }
        },
        methods: {
            productView() {

            }
        }
    }
</script>

<template>
    <div class="px-3">
        <h2 class="text-3xl text-gray-100 font-bold text-center underline">Our Shop</h2>
        <div class="flex flex-wrap">
            <div class="m-auto" v-for="(value, key) in products">
                <div class="bg-gray-200 p-4 m-3">
                    <button>
                        <p>{{ key }}</p>
                        <div>
                            <img :src="value.image" alt="">
                        </div>
                        <h3>{{ value.name }}</h3>
                        <h4>{{ value.price }}</h4>
                    </button>
                </div>
            </div>
        </div>
    </div>
</template>