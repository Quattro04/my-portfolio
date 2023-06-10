<template>
    <div class="mx-auto mb-auto mt-64 xl:mr-auto xl:ml-0">
        <h1 class="xl:ml-64 text-4xl xl:text-7xl text-white tracking-widest text-center">Matija Jeras</h1>
        <h2 class="xl:ml-64 mt-4 pl-1 xl:text-xl text-white tracking-wider px-3 text-center">Software developer with passion for front-end</h2>
    </div>
    <div class="absolute left-1/2 top-28 xl:top-1/2 xl:left-auto xl:right-0 transform -translate-x-1/2 xl:-translate-y-1/2 xl:translate-x-0">
        <img v-if="isDesktop" id="logo" class="next-particle hidden"
            data-init-position="random"
            data-init-direction="random"
            data-fade-position="random"
            data-fade-direction="random"

            data-particle-gap="2"

            data-width="900"
            data-height="700"                

            data-mouse-force="60"

            data-gravity="0.3"

            data-noise="40"
            src="/logo_white_square.png"
            data-not-lazy
        />
        <img v-if="!isDesktop" id="logo" class="next-particle hidden"
            data-init-position="random"
            data-init-direction="random"
            data-fade-position="random"
            data-fade-direction="random"

            data-particle-gap="2"

            data-width="300"
            data-height="200"                

            data-mouse-force="60"

            data-gravity="0.3"

            data-noise="40"
            src="/logo_white_square.png"
            data-not-lazy
        />
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
<script>
export default {
    data() {
        return {
            isLoaded: false
        }
    },
    computed: {
        isDesktop() {
            if (typeof window === 'undefined') {
                return false;
            }
            return window.innerWidth > 1279;
        }  
    },
    mounted() {
        new NextParticle(document.all.logo);
    }
}
</script>

<style lang="css">
body {
    font-family: 'Poppins', sans-serif;
    font-family: 'Varela Round', sans-serif;
}
</style>
