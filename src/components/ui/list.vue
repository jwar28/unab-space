<script setup>
const props = defineProps({
    arrayToDisplay: Array
})
</script>

<template>
    <div class="grid sm:grid-cols-2 md:grid-cols-3 mt-16 gap-16 justify-center">
        <div class="flex gap-4 items-start" v-for="(item, index) in arrayToDisplay" :key="index">
            <div>
                <h3 class="font-semibold text-lg text-center">{{ item.title }}</h3>
                <p class="text-slate-600 mt-2 leading-relaxed text-justify">
                    {{ item.description }}
                </p>
            </div>
        </div>
    </div>
</template>