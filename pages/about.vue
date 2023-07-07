<template>
    <div class="flex flex-col p-10 xl:mx-96 xl:p-0 items-center">
        <span class="text-teal-300 text-xl xl:text-3xl mb-5">Hey, I'm Matija</span>
        <Transition>
            <span v-if="showFirst" class="text-slate-200 text-md xl:text-xl text-center mb-5">Software developer focused on frontend code that enables me to program a clean and intuitive web based applications. I'm always looking for new challenges and don't like to stagnate by doing easy repetitive work.</span>
        </Transition>
        <Transition>
            <span v-if="showSeparator" class="w-full h-0.5 bg-teal-500 mb-5"></span>
        </Transition>
        <Transition>
            <span  v-if="showSecond" class="text-slate-200 text-md xl:text-xl text-center">With 8+ years of experience in the industry, I have developed a strong foundation in both front-end and back-end development. I've been focused primarily on front-end, I am proficient in using React with Next.js to create intuitive, responsive and visually appealing web applications, while also taking care of server-side rendering and optimized SEO.</span>
        </Transition>
    </div>
</template>
<script>
export default {
    data() {
        return {
            showTitle: false,
            showFirst: false,
            showSeparator: false,
            showSecond: false
        }
    },
    mounted() {
        setTimeout(() => {
            this.showTitle = true;
        }, 1)
        setTimeout(() => {
            this.showFirst = true;
        }, 1000)
        setTimeout(() => {
            this.showSeparator = true;
        }, 2000)
        setTimeout(() => {
            this.showSecond = true;
        }, 2000)
    }
}
</script>
<style>
.v-enter-to,
.v-leave-from {
  opacity: 1;
}

.v-enter-active,
.v-leave-active {
  transition: all 0.5s ease;
}

.v-enter-from,
.v-leave-to {
  opacity: 0;
}
</style>