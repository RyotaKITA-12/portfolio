<template>
    <div v-show="loading">
        <div class="fullview">
            <div class="loading-spacer"></div>
            <vue-loading type="spiningDubbles" color="#64c8aa" :size="{ width: '5%', height: '10%' }" />
        </div>
    </div>
</template>

<script>
import { VueLoading } from 'vue-loading-template'

export default {
    name: 'loading',
    components: {
        VueLoading,
    },
}
</script>

<style>
.fullview {
    width: 100%;
    height: 100%;
    position: fixed;
    top: 0;
    left: 0;
}

.loading-spacer {
    height: 40%;
}
</style>
