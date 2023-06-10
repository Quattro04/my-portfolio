<template>
    <div class="flex flex-1 py-20 px-32 h-full">
        <VueWordCloud :words="words" :spacing="1"/>
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
                { text: 'React', weight: 90, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'Next', weight: 80, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'Vue', weight: 70, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'Nuxt', weight: 50, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'Angular', weight: 50, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'Node', weight: 90, fontFamily: "'Varela Round', sans-serif", color: '#93c5fd' },
                { text: 'CSS', weight: 95, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'SASS', weight: 70, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'LESS', weight: 50, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'Tailwind', weight: 80, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'Bulma', weight: 60, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'Semantic', weight: 60, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'Javascript', weight: 80, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'Typescript', weight: 90, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'HTML', weight: 95, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'Python', weight: 50, fontFamily: "'Varela Round', sans-serif", color: '#93c5fd' },
                { text: 'Java', weight: 30, fontFamily: "'Varela Round', sans-serif", color: '#93c5fd' },
                { text: 'PHP', weight: 20, fontFamily: "'Varela Round', sans-serif", color: '#93c5fd' },
                { text: 'Laravel', weight: 30, fontFamily: "'Varela Round', sans-serif", color: '#93c5fd' },
                { text: 'Jira', weight: 60, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'Git', weight: 90, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'SQL', weight: 10, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'mongoDB', weight: 50, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'PlanetScale', weight: 60, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'Prisma', weight: 55, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'Photoshop', weight: 80, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
                { text: 'Golang', weight: 70, fontFamily: "'Varela Round', sans-serif", color: '#93c5fd' },
                { text: 'Pixi.js', weight: 40, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'Three.js', weight: 60, fontFamily: "'Varela Round', sans-serif", color: '#2dd4bf' },
                { text: 'Blender', weight: 20, fontFamily: "'Varela Round', sans-serif", color: '#e2e8f0' },
            ]
        }
    }
}
</script>
<style lang="css">
</style>