<template>
    <div class="h-screen flex flex-col bg-gradient-to-r from-emerald-600 to-blue-600 overflow-hidden">
        <Navigation />
        <NuxtLayout>
            <NuxtPage />
        </NuxtLayout>
        <Socials />
    </div>
</template>
<script setup>
    useHead({
        link: [
            { href: 'https://fonts.googleapis.com', rel: 'preconnect' },
            { href: 'https://fonts.gstatic.com', rel: 'preconnect', crossorigin: true },
            { href: 'https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;700&family=Varela+Round&display=swap', rel: 'stylesheet' },
        ],
        script: [{ src: "/nextparticle.js", type: "text/javascript" }],
    });
</script>
