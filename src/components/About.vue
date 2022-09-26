<template>
    <v-app>
        <v-parallax height="400" :src="require('@/assets/about/background.png')">
            <v-row align="center" justify="center">
                <v-col class="text-center" cols="12">
                    <h1 class="text-h4 font-weight-thin mb-4">
                        <b>Ryota KITA</b>
                    </h1>
                    <h4 class="subheading">
                        E N G I N E E R I N G　|　D E S I G N
                    </h4>
                </v-col>
            </v-row>
        </v-parallax>
    </v-app>
</template>

<script>
export default {
    data: () => ({
    })
}
</script>
<style>
.bakcground {
    background-image: url("~@/assets/about/background.png");
    background-size: cover;
}
</style>
