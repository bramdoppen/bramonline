<template>
    <header>
        <div class="container mx-auto">
            <div class="flex py-6 justify-between items-center">
                <div class="flex flex-row gap-8 items-center">
                    <NuxtLink to="/">
                        <p class="text-body-lg font-bold text-neutral-900">
                            Bram Doppen
                        </p>
                    </NuxtLink>
                </div>
                <div class="flex flex-row gap-6">
                    <div class="md:flex hidden flex-row gap-6 items-center">

                        <NuxtLink v-for="item in navigation" :key="item.name" :to="item.href"
                            class="text-body-sm font-medium text-neutral-700 hover:text-primary-600 px-4">
                            {{ item.name }}
                        </NuxtLink>

                    </div>
                    <Button label="CONTACT" link="#" />
                </div>
            </div>
        </div>
    </header>
</template>

<script setup>
const navigation = ref([
    { name: "Work", href: "#work" },
    { name: "Services", href: "#services" },
    { name: "About", href: "#about" },
])
</script>

