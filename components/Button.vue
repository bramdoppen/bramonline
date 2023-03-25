

<template>
    <NuxtLink class="button flex items-center justify-center rounded-full bg-primary-600 text-white font-semibold"
        :class="size === 'lg' ? 'px-6 py-4 text-body-sm' : 'px-4 py-2.5 text-body-xs'" :to="link">
        {{ label }}
    </NuxtLink>
</template>

<script setup>
const props = defineProps(['link', 'label'])
</script>