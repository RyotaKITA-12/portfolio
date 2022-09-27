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
        <div style="height: 5%;" />
        <v-row justify="center">
            <v-col cols=9>
                <v-card color="#121212" outlined tile>
                    <v-card-title class="text-h4">
                        EDUCATION
                    </v-card-title>
                    <br>
                    <v-card-subtitle>
                        <p class="text-h5"><b>Chubu University Daiichi High School</b></p>
                        <p class="text-h6">Electrical and Electronic Systems</p>
                    </v-card-subtitle>
                    <v-card-text>
                        電気電子・情報分野の資格・検定を30個ほど取得し、愛知県高等学校職業教育技術認定事業グランプリを受賞
                    </v-card-text>
                    <br>
                    <v-card-subtitle>
                        <p class="text-h5"><b>Musashino University</b></p>
                        <p class="text-h6">Data Science</p>
                    </v-card-subtitle>
                    <v-card-text>
                        ゼミや有志PJでの研究活動，学外ハッカソンを中心に活動．
                        特に，ハッカソンでは数多くの賞を受賞．
                        <br>
                        また，学内交流会や勉強会を数多く企画・運営している．
                    </v-card-text>
                </v-card>
            </v-col>
        </v-row>
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
