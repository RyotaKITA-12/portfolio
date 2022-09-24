<template>
    <v-app id="inspire">
        <v-app-bar app flat>
            <v-tabs centered class="ml-n9" color="cyan lighten-2">
                <v-tab v-for="link in links" :key="link">
                    {{ link }}
                </v-tab>
            </v-tabs>

        </v-app-bar>

        <v-main>
            <v-container>

            </v-container>
        </v-main>
    </v-app>
</template>

<script>
export default {
    name: 'Home',
    data: () => ({
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
