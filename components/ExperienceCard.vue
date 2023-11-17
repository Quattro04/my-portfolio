<template>
    <flip-card>
        <template #front>
            <div :class="`
                group
                flex-1 flex flex-col h-44 py-8 px-10 m-5 rounded-xl bg-white
                drop-shadow cursor-pointer relative overflow-hidden
            `">
                <span class="uppercase font-semibold text-sky-700">
                    {{ company }}
                </span>
                <span class="mt-2">
                    {{ position }}
                </span>
                <span class="text-zinc-400 mt-auto">
                    {{ duration }}
                </span>
                <div :class="`
                    ${'queue-'+queue}
                    absolute top-0 right-0 w-6 h-full flex items-center justify-center translate-x-5 transition-transform
                    group-hover:translate-x-0
                `">
                    <svg width="50px" height="50px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M10 7L15 12L10 17" stroke="#FFFFFF" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                    </svg>
                </div>
            </div>
        </template>
        <template #back>
            <div :class="`
                flex-1 flex flex-col h-44 py-4 px-4 m-5 rounded-xl bg-white
                drop-shadow cursor-pointer relative overflow-hidden\
            `">
                <slot />
            </div>
        </template>
    </flip-card>
</template>
<script>
    export default {
        name: 'experience-card',
        props: ['company', 'position', 'duration', 'queue']
    }
</script>
<style>
.queue-2,
.queue-2 {
    background-color: #0c4a6e;
    /* background-color: #7dd3fc; */
}
.queue-4,
.queue-4 {
    background-color: #0369a1;
    /* background-color: #0ea5e9; */
}
.queue-6,
.queue-6 {
    background-color: #0ea5e9;
    /* background-color: #0369a1; */
}
.queue-8,
.queue-8 {
    background-color: #7dd3fc;
    /* background-color: #0c4a6e; */
}
</style>
