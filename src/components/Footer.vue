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
        <div class="flex flex-col py-2 bg-slate-300 mb-2 box-shadow">
            <div>
                <p class="text-lg text-center text-gray-950">{{ text }}</p>
            </div>
        </div>
    </footer>
</template>