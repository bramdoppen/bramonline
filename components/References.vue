<template>
    <div>
        <div class="container mx-auto">
            <div class="md:py-12 py-8">
                <div class="flex justify-center relative pb-1">
                    <span class="absolute block h-px bg-white bottom-1/2 left-0 right-0 bg-logo-clouds-line"></span>
                    <div class="bg-white px-6 py-3 relative">
                        <p class="text-body-sm font-semibold tracking-2 text-neutral-500">
                            CRAFTED DESIGNS FOR
                        </p>
                    </div>
                </div>
                <div class="flex flex-row flex-wrap justify-center items-center gap-8 py-6">
                    {data.clients.edges.map(({ node }) => (
                    <img src={node.publicURL} alt={node.name} key={node.id} />
                    ))}
                </div>
                <div class="flex justify-center relative pb-1">
                    <span class="absolute block h-px bg-white bottom-1/2 left-0 right-0 bg-logo-clouds-line"></span>
                    <div class="bg-white px-6 py-3 relative">
                        <p class="text-body-sm font-semibold tracking-2 text-neutral-500">
                            MORE THAN 150+ BRANDS
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>