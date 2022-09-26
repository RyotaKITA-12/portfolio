<template>
    <v-app>
        <cursor-fx color="#4DD0E1" color-hover="#acf98e" />
        <Loading v-show="loading" />
        <Home v-show="!loading" />
    </v-app>
</template>

<script>

import Loading from '@/components/Loading'
import Home from '@/views/Home'

export default {
    name: 'App',
    components: {
        Loading,
        Home,
    },
    data: () => ({
        loading: true,
    }),
    mounted() {
        setTimeout(() => {
            this.loading = false
        }, 700)
    }
};
</script>
