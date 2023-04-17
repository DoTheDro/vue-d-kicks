<script>
    import product1 from '../assets/images/adidas-shoe-sneakers.png'
    import product2 from '../assets/images/adidas-yeezy.png'
    import product3 from '../assets/images/nike-air-max.png'
    import product4 from '../assets/images/shoe-nike-air-max.png'
    import product5 from '../assets/images/sneaker-nike-shoe.png'
    import product6 from '../assets/images/sneakers-adidas-stan-smith.png'
    import product7 from '../assets/images/sneakers-basketball.png'
    import product8 from '../assets/images/sneakers-skate-shoe.png'
    import product9 from '../assets/images/vans-old-skool.png'
    import product10 from '../assets/images/vans-skate-shoe-fire.png'
    import product11 from '../assets/images/vans-skate-shoe.png'
    import product12 from '../assets/images/vans-slip-on-shoe.png'
    import Modal from './Modal.vue'

    export default {
        components: { Modal },
        data() {
            return {
                products: [
                    { name: 'Adidas Sneaker', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: product1, price: '187.00', brand: 'adidas' },
                    { name: 'Yeezy', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: product2, price: '135.00', brand: 'adidas' },
                    { name: 'Air Max', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: product3, price: '150.00', brand: 'nike' },
                    { name: 'Air Max Zoom', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: product4, price: '198.00', brand: 'nike' },
                    { name: 'Nike Sneaker', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: product5, price: '186.00', brand: 'nike' },
                    { name: 'Sneaker Stan Smith', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: product6, price: '108.00', brand: 'adidas' },
                    { name: 'Sneaker', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: product7, price: '200.00', brand: 'nike' },
                    { name: 'Adidas Skater', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: product8, price: '107.00', brand: 'adidas' },
                    { name: 'Old Skool', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: product9, price: '101.00', brand: 'vans' },
                    { name: 'Skater - Fire', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: product10, price: '192.00', brand: 'vans' },
                    { name: 'Vans Skater', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: product11, price: '147.00', brand: 'vans' },
                    { name: 'Vans Slip-on', description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Optio esse eveniet eaque possimus, laboriosam magnam!', image: product12, price: '108.00', brand: 'vans' },
                ],
                show: false,
                itemShowcase: ''
            }
        },
        methods: {
            productView(key) {
                this.itemShowcase = this.products[key]
                this.show = !this.show
            },
            closeModal() {
                this.show = !this.show
            }
        }
    }
</script>

<template>
    <div class="ease-in duration-500" v-if="show">
        <Modal :content="itemShowcase" @close="closeModal" />
    </div>
    <div data-aos="fade-down"
        data-aos-duration="700"
        data-aos-once="true"
    class="px-3 flex flex-col gap-5 mb-28" id="shop">
        <h2 class="text-3xl text-gray-100 font-bold text-center underline">Our Shop</h2>
        <p class="text-lg text-gray-100 text-center">Lorem, ipsum dolor.</p>
        <div class="flex flex-wrap md:max-w-5xl md:m-auto">
            <div class="m-auto sm:w-6/12 sm:box-shadow md:w-2/6" v-for="(value, key) in products">
                <div class="bg-gray-200 p-6 m-3 custom-min-height-sm flex rounded-lg sm:box-shadow md:hover:scale-110 md:duration-500 md:hover:box-shadow">
                    <button class="flex flex-col justify-between items-center" @click="productView(key)">
                        <div class="max-w-xs">
                            <img :src="value.image" alt="">
                        </div>
                        <div class="flex flex-col gap-4">
                            <h3 class="text-2xl font-bold">{{ value.name }}</h3>
                            <h4 class="text-lg font-medium">$ {{ value.price }}</h4>
                        </div>
                    </button>
                </div>
            </div>
        </div>
    </div>
</template>