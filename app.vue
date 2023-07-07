<template>
    <div class="h-screen flex">
        <div class="flex-[0_0_300px] flex flex-col items-center justify-around bg-white">
            <img class="w-24 h-24 rounded-full" src="logo_square.png" />
            <Navigation />
            <Socials />
        </div>
        <div class="flex-1 flex flex-col bg-sky-100 rounded-l-3xl py-14 px-16 drop-shadow">
            <NuxtPage />
        </div>
    </div>
</template>
<script setup>
    useHead({
        link: [
            { href: 'https://fonts.googleapis.com', rel: 'preconnect' },
            { href: 'https://fonts.gstatic.com', rel: 'preconnect', crossorigin: true },
            { href: 'https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;700&family=Varela+Round&display=swap', rel: 'stylesheet' },
        ],
    });
</script>
