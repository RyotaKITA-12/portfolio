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
            <v-container style="padding: 25px;">
                <Skills v-if="page === 'SKILLS'" />
                <Works v-if="page === 'WORKS'" />
            </v-container>
        </v-main>
    </v-app>
</template>

<script>
import Skills from '@/components/Skills'
import Works from '@/components/Works'

export default {
    name: 'Home',
    components: {
        Skills,
        Works,
    },
    data: () => ({
        page: "ABOUT",
        links: [
            'ABOUT',
            'ACTIVITY',
            'NEWS',
            'SKILLS',
            'WORKS',
        ],
    }),
}
</script>
