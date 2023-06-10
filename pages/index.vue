<template>
    <div>
        <h1 class="ml-64 text-7xl text-white tracking-widest">Matija Jeras</h1>
        <h2 class="ml-64 mt-4 pl-1 text-xl text-white tracking-wider">Software developer with passion for front-end</h2>
        <div class="absolute right-0 top-1/2 transform -translate-y-1/2">
            <img id="logo" class="next-particle hidden"
                data-init-position="random"
                data-init-direction="random"
                data-fade-position="random"
                data-fade-direction="random"

                data-particle-gap="2"

                data-width="900"
                data-height="700"

                data-max-width="700"
                data-max-height="500"                    

                data-mouse-force="60"

                data-gravity="0.3"

                data-noise="40"
                src="/logo_white_square.png"
                data-not-lazy
            />
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
        script: [{ src: "/nextparticle.js", type: "text/javascript", async: true, nonce: true }],
    });
</script>
<script>
export default {
    data() {
        return {
            isLoaded: false
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
