<template>
    <nav class="flex flex-col w-full px-14 font-semibold text-sm text-zinc-700">
        <NuxtLink to="/" class="router-link flex items-center justify-center m-3 py-5 rounded-xl">
            <span>Home</span>
        </NuxtLink>
        <NuxtLink to="/skills" class="router-link flex items-center justify-center m-3 py-5 rounded-xl">
            <span>Skills</span>
        </NuxtLink>
        <NuxtLink to="/about" class="router-link flex items-center justify-center m-3 py-5 rounded-xl">
            <span>About</span>
        </NuxtLink>
        <NuxtLink to="/cv" class="router-link flex items-center justify-center m-3 py-5 rounded-xl">
            <span>CV</span>
        </NuxtLink>
    </nav>
</template>
<style>
.router-link {
    transition: 0.5s linear;
    box-shadow: 2px 2px 5px 0px rgba(0,0,0,0.1);
}

/* .router-link span {
    transition: 0.5s;
}
.router-link:hover span {
    transform: translateY(-30%);
}
.router-link-active {
    opacity: 0.4;
    pointer-events: none;
} */
</style>