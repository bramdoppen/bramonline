<template>
    <footer class="bg-black text-white">
        <div class="container mx-auto">
            <div class="flex flex-col md:py-30 pt-12 pb-20 md:gap-24 gap-16">
                <div>
                    <h3 class="md:text-display-xl text-display-md font-semibold pb-4">
                        Heb je een idee?
                    </h3>
                    <a href="https://www.linkedin.com/in/bramdoppen/" target="_blank"
                        class="md:text-display-xl text-display-md font-normal hover:text-primary-100 hover:underline">
                        Let’s talk ↗
                    </a>
                </div>
                <div class="flex md:flex-row flex-col md:gap-8 gap-12 justify-between">
                    <div>
                        <a href="mailto:sites@bram.onl"
                            class="md:text-display-xs text-body-xl font-medium text-neutral-200 hover:text-primary-100 hover:underline">
                            sites@bram.onl
                        </a>
                    </div>
                    <div class="grid md:grid-cols-3 grid-cols-2 md:gap-12 gap-3 md:pl-32">
                        <a v-for="item in social" :key="item.name" :href="item.href" :target="item.target"
                            class="md:text-body-xl text-body-md font-normal text-neutral-200 hover:text-primary-100">
                            {{ item.name }}
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script setup>
const social = ref([
    { name: "Mail", href: "mailto:sites@bram.onl", target: "_self" },
    { name: "Github", href: "https://www.github.com/bramdoppen/", target: "_blank" },
    { name: "LinkedIn", href: "https://www.linkedin.com/in/bramdoppen/", target: "_blank" },
]);
</script>
