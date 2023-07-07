<template>
    <div class="cont flex flex-col xl:my-10 py-3 px-4 mx-3 xl:py-6 xl:px-8 rounded-xl">
        <div class="flex items-center justify-between">
            <div class="flex items-center">
                <i class="w-3 h-3 bg-teal-300 mr-2 border border-black"></i>
                <span class="text-slate-200">Frontend</span>
            </div>
            <div class="flex items-center">
                <div class="w-3 h-3 bg-sky-400 mr-2 border border-black"></div>
                <span class="text-slate-200">Backend</span>
            </div>
            <div class="flex items-center">
                <div class="w-3 h-3 bg-slate-200 mr-2 border border-black"></div>
                <span class="text-slate-200">Other</span>
            </div>
        </div>
        <div class="text-slate-200 mt-2 text-center">
            Larger font means more experience with that technology
        </div>
    </div>
    <div class="flex flex-1 w-full py-3 px-4 xl:pb-20 xl:px-32 h-full">
        <VueWordCloud :words="words" :spacing="1" />
    </div>
</template>
<script>
import VueWordCloud from "vuewordcloud";
export default {
    components: {
        VueWordCloud,
    },
    data() {
        return {
            words: [
                { text: 'React', weight: 90, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'Next', weight: 80, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'Vue', weight: 70, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'Nuxt', weight: 50, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'Angular', weight: 50, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'Node', weight: 90, fontFamily: "'Varela Round', sans-serif", color: '#38bdf8' },
                { text: 'CSS', weight: 95, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'SASS', weight: 70, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'LESS', weight: 50, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'Tailwind', weight: 80, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'Bulma', weight: 60, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'Semantic', weight: 60, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'Javascript', weight: 80, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'Typescript', weight: 90, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'HTML', weight: 95, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'Python', weight: 50, fontFamily: "'Varela Round', sans-serif", color: '#38bdf8' },
                { text: 'Java', weight: 30, fontFamily: "'Varela Round', sans-serif", color: '#38bdf8' },
                { text: 'PHP', weight: 20, fontFamily: "'Varela Round', sans-serif", color: '#38bdf8' },
                { text: 'Laravel', weight: 30, fontFamily: "'Varela Round', sans-serif", color: '#38bdf8' },
                { text: 'Jira', weight: 60, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'Git', weight: 90, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'SQL', weight: 10, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'mongoDB', weight: 50, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'PlanetScale', weight: 60, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'Prisma', weight: 55, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'Photoshop', weight: 80, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'Golang', weight: 70, fontFamily: "'Varela Round', sans-serif", color: '#38bdf8' },
                { text: 'Pixi.js', weight: 40, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'Three.js', weight: 60, fontFamily: "'Varela Round', sans-serif", color: '#5eead4' },
                { text: 'Blender', weight: 20, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
            ]
        }
    }
}
</script>
<style lang="css">
.cont {
    background-color: rgba(0,0,0,0.2);
}
</style>