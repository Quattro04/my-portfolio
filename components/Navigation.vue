<template>
    <nav class="w-full h-24 justify-around xl:justify-center flex text-md text-white no-print">
        <NuxtLink to="/" class="router-link flex items-center xl:px-10 tracking-wide"><span>HOME</span></NuxtLink>
        <NuxtLink to="/skills" class="router-link flex items-center xl:px-10 tracking-wide"><span>SKILLS</span></NuxtLink>
        <NuxtLink to="/about" class="router-link flex items-center xl:px-10 tracking-wide"><span>ABOUT</span></NuxtLink>
        <!-- <NuxtLink to="/blog" class="link px-10">Blog</NuxtLink> -->
        <NuxtLink to="/cv" class="router-link flex items-center xl:px-10 tracking-wide"><span>CV</span></NuxtLink>
    </nav>
</template>
<style>
.router-link span {
    transition: 0.5s;
}
.router-link:hover span {
    transform: translateY(-30%);
}
.router-link-active {
    opacity: 0.4;
    pointer-events: none;
}
</style>