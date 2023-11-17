<template>
    <div :class="`absolute w-60 h-screen ${opened ? 'left-0' : '-left-full'} top-0 flex flex-col items-center justify-around bg-white z-10`">
        <img class="w-24 h-24 rounded-full" src="logo_square.png" />
        <Navigation />
        <Socials />
    </div>
</template>
<script>
    export default {
        name: 'side-menu',
        props: ['opened']
    }
</script>