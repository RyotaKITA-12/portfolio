<template>
    <v-app id="inspire">
        <v-app-bar app flat>
            <v-tabs centered class="ml-n9" color="cyan lighten-2">
                <v-tab v-for="link in links" :key="link" @click="page = link">
                    {{ link }}
                </v-tab>
            </v-tabs>

        </v-app-bar>

        <v-main>
            <div v-if="page === 'ABOUT'">
                <About />
            </div>
            <div v-else>
                <v-container style="padding: 25px;">
                    <News v-if="page === 'NEWS'" />
                    <Skills v-if="page === 'SKILLS'" />
                    <Works v-if="page === 'WORKS'" />
                </v-container>
            </div>
        </v-main>
    </v-app>
</template>

<script>
import About from '@/components/About'
import News from '@/components/News'
import Skills from '@/components/Skills'
import Works from '@/components/Works'

export default {
    name: 'Home',
    components: {
        About,
        News,
        Skills,
        Works,
    },
    data: () => ({
        page: "ABOUT",
        links: [
            'ABOUT',
            'NEWS',
            'SKILLS',
            'WORKS',
        ],
    }),
}
</script>
