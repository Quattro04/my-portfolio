<template>
    <div class="group flex-[0_0_200px] flex flex-col h-48 m-5 rounded-xl bg-white drop-shadow cursor-pointer relative overflow-hidden">
        <div class="h-12 py-3 px-5 text-white text-center rounded-t-xl relative" :class="titleAsClass">
            <span class="flex items-center transition absolute top-1/2 left-0 transform -translate-x-full -translate-y-1/2 group-hover:left-1/2 group-hover:-translate-x-1/2">
                More info
                <svg class="ml-1" width="16px" height="16px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill="#ffffff" fill-rule="evenodd" clip-rule="evenodd" d="M12.2929 4.29289C12.6834 3.90237 13.3166 3.90237 13.7071 4.29289L20.7071 11.2929C21.0976 11.6834 21.0976 12.3166 20.7071 12.7071L13.7071 19.7071C13.3166 20.0976 12.6834 20.0976 12.2929 19.7071C11.9024 19.3166 11.9024 18.6834 12.2929 18.2929L17.5858 13H4C3.44772 13 3 12.5523 3 12C3 11.4477 3.44772 11 4 11H17.5858L12.2929 5.70711C11.9024 5.31658 11.9024 4.68342 12.2929 4.29289Z"/></svg>
            </span>
            <span class="transition absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 group-hover:hidden group-hover:translate-x-0">
                {{ title }}
            </span>
        </div>
        <div class="flex-1 w-full flex items-center justify-center">
            <slot />
            <div class="absolute bottom-0 h-1 w-full rounded-b-xl transition transform translate-y-full group-hover:translate-y-0" :class="titleAsClass" />
        </div>
    </div>
</template>
<script>
    export default {
        name: 'skill-card',
        props: ['title'],
        computed: {
            titleAsClass() {
                return this.title.replace('.', '').replace(' ', '').toLowerCase()
            }
        }
    }
</script>
<style>
.nextjs {
    background-color: black;
}
.nuxtjs {
    background-color: #41b883;
}
.tailwindcss {
    background-color: #06b6d4;
}
.testing {
    background-color: #a91f75;
}
.photoshop {
    background-color: #0a5991;
}
</style>
