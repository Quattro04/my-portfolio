<template>
    <flip-card>
        <template #front>
            <div :class="`
                ${'queue-'+queue}
                flex-1 flex flex-col h-44 py-8 px-10 mx-10 ml-0 rounded-xl bg-white
                drop-shadow cursor-pointer relative overflow-hidden
                before:content-[''] before:absolute before:right-0 before:top-0 before:w-1 before:h-1/2 before:origin-bottom before:transition-all
                hover:before:-rotate-45 hover:before:h-4 hover:before:w-1 hover:before:top-1/2 hover:before:-translate-y-full hover:before:rounded-xl hover:before:mt-0.5 hover:before:mr-2
                after:content-[''] after:absolute after:right-0 after:bottom-0 after:w-1 after:h-1/2 after:origin-top after:transition-all
                hover:after:rotate-45 hover:after:h-4 hover:after:w-1 hover:after:bottom-1/2 hover:after:translate-y-full hover:after:rounded-xl hover:after:mr-2
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
            </div>
        </template>
        <template #back>
            <div :class="`
                ${'queue-'+queue}
                flex-1 flex flex-col h-44 py-4 pl-4 pr-5 mx-10 ml-0 rounded-xl bg-white
                drop-shadow cursor-pointer relative overflow-hidden
                before:content-[''] before:absolute before:right-0 before:top-0 before:w-1 before:h-1/2 before:origin-bottom before:transition-all
                hover:before:-rotate-45 hover:before:h-4 hover:before:w-1 hover:before:top-1/2 hover:before:-translate-y-full hover:before:rounded-xl hover:before:mt-0.5 hover:before:mr-2
                after:content-[''] after:absolute after:right-0 after:bottom-0 after:w-1 after:h-1/2 after:origin-top after:transition-all
                hover:after:rotate-45 hover:after:h-4 hover:after:w-1 hover:after:bottom-1/2 hover:after:translate-y-full hover:after:rounded-xl hover:after:mr-2
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
.queue-2:before,
.queue-2:after {
    background-color: #0c4a6e;
    /* background-color: #7dd3fc; */
}
.queue-4:before,
.queue-4:after {
    background-color: #0369a1;
    /* background-color: #0ea5e9; */
}
.queue-6:before,
.queue-6:after {
    background-color: #0ea5e9;
    /* background-color: #0369a1; */
}
.queue-8:before,
.queue-8:after {
    background-color: #7dd3fc;
    /* background-color: #0c4a6e; */
}
</style>
