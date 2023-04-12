<script>
    export default {
        data() {
            return {
                text: 'Created and built by Andrew Buhat'
            }
        }
    }
</script>

<template>
    <footer>
        <div class="flex flex-col py-5 bg-slate-300 mb-4 box-shadow">
            <div>
                <p class="text-lg text-center text-gray-950">{{ text }}</p>
            </div>
        </div>
    </footer>
</template>