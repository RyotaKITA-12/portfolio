<template>
    <v-app>
        <div style="margin-top: 40px; margin-bottom: 20px;">
            <p class="text-h5 font-weight-bold cyan--text">2022</p>
            <v-divider color="cyan" />
        </div>
        <v-row align-content="center">
            <div v-for="content in contents2022" :key="content">
                <v-col>
                    <v-card height="250" width="265" :color="content.color">
                        <v-img :src="require(`@/assets/works/${content.image}`)" contain="true" height="155" />
                        <v-card-title>
                            <v-icon style="margin-right: 10px; margin-left: -5px; margin-top: -7px;">
                                {{ content.icon }}
                            </v-icon>
                            {{ content.title }}
                        </v-card-title>
                        <v-card-subtitle> {{ content.story }} </v-card-subtitle>
                    </v-card>
                </v-col>
            </div>
        </v-row>
        <div style="margin-top: 40px; margin-bottom: 20px;">
            <p class="text-h5 font-weight-bold cyan--text">2021</p>
            <v-divider color="cyan" />
        </div>
        <v-row align-content="center">
            <div v-for="content in contents2021" :key="content">
                <v-col>
                    <v-card height="250" width="265" :color="content.color">
                        <v-img :src="require(`@/assets/works/${content.image}`)" contain="true" height="155" />
                        <v-card-title>
                            <v-icon style="margin-right: 10px; margin-left: -5px; margin-top: -7px;">
                                {{ content.icon }}
                            </v-icon>
                            {{ content.title }}
                        </v-card-title>
                        <v-card-subtitle> {{ content.story }} </v-card-subtitle>
                    </v-card>
                </v-col>
            </div>
        </v-row>
        <div style="margin-top: 40px; margin-bottom: 20px;">
            <p class="text-h5 font-weight-bold cyan--text">2020</p>
            <v-divider color="cyan" />
        </div>
        <v-row align-content="center">
            <div v-for="content in contents2020" :key="content">
                <v-col>
                    <v-card height="250" width="265" :color="content.color">
                        <v-img :src="require(`@/assets/works/${content.image}`)" contain="true" height="155" />
                        <v-card-title>
                            <v-icon style="margin-right: 10px; margin-left: -5px; margin-top: -7px;">
                                {{ content.icon }}
                            </v-icon>
                            {{ content.title }}
                        </v-card-title>
                        <v-card-subtitle> {{ content.story }} </v-card-subtitle>
                    </v-card>
                </v-col>
            </div>
        </v-row>
        <div style="margin-top: 40px; margin-bottom: 20px;">
            <p class="text-h5 font-weight-bold cyan--text">2019</p>
            <v-divider color="cyan" />
        </div>
        <v-row align-content="center">
            <div v-for="content in contents2019" :key="content">
                <v-col>
                    <v-card height="250" width="265" :color="content.color">
                        <v-img :src="require(`@/assets/works/${content.image}`)" contain="true" height="155" />
                        <v-card-title>
                            <v-icon style="margin-right: 10px; margin-left: -5px; margin-top: -7px;">
                                {{ content.icon }}
                            </v-icon>
                            {{ content.title }}
                        </v-card-title>
                        <v-card-subtitle> {{ content.story }} </v-card-subtitle>
                    </v-card>
                </v-col>
            </div>
        </v-row>
    </v-app>
</template>

<script>
export default {
    data: () => ({
        contents2022: [
            {
                title: "CurriCreate",
                story: "データベースデザイン 課題",
                image: "curriculum.png",
                icon: "mdi-school",
                color: "indigo darken-1",
            },
            {
                title: "FU-CALENDAR",
                story: "技育展2022 (株式会社サポーターズ)",
                image: "fu-calendar.png",
                icon: "mdi-calendar",
                color: "indigo darken-1",
            },
            {
                title: "preGen",
                story: "技育CAMP オンライン開発合宿 ...",
                image: "pregen.png",
                icon: "mdi-presentation",
                color: "indigo darken-1",
            },
            {
                title: "Hack-a-Matcher",
                story: "技育CAMP オンライン開発合宿 ...",
                image: "hack-a-matcher.png",
                icon: "mdi-link-variant",
                color: "indigo darken-1",
            },
            {
                title: "FU CALENDAR",
                story: "技育CAMP オンライン開発合宿 ...",
                image: "fucalendar.png",
                icon: "mdi-calendar",
                color: "indigo darken-1",
            },
        ],
        contents2021: [
            {
                title: "Gazeat",
                story: "Open Hack U 2021 Online Vol.4",
                image: "gazeat.png",
                icon: "mdi-puzzle",
                color: "indigo darken-1",
            },
            {
                title: "ソースコードの構文...",
                story: "DEIM2022 第14回データ工学と情...",
                image: "tree.png",
                icon: "mdi-xml",
                color: "teal darken-1",
            },
            {
                title: "カッコウ探索アルゴ...",
                story: "情報処理学会 第84回全国大会",
                image: "cuckoo.png",
                icon: "mdi-bird",
                color: "teal darken-1",
            },
            {
                title: "もぐもぐ",
                story: "技育CAMP オンライン開発合宿 ...",
                image: "mogumogu.png",
                icon: "mdi-food",
                color: "indigo darken-1",
            },
            {
                title: "金魚すくわれ",
                story: "お盆deハッカソン (株式会社 TeckB...",
                image: "kingyo.png",
                icon: "mdi-fish",
                color: "indigo darken-1",
            },
            {
                title: "筋トレドリーム",
                story: "技育CAMP オンライン開発合宿 ...",
                image: "pushup.png",
                icon: "mdi-weight-lifter",
                color: "indigo darken-1",
            },
        ],
        contents2020: [
            {
                title: "テキストデータを対...",
                story: "情報処理学会 第83回全国大会",
                image: "opinion.png",
                icon: "mdi-message-processing",
                color: "teal darken-1",
            },
            {
                title: "共起ネットワークを...",
                story: "武蔵野大学オープンキャンパス202...",
                image: "covid.png",
                icon: "mdi-share-variant",
                color: "teal darken-1",
            },
        ],
        contents2019: [
            {
                title: "MESHを用いた文化祭...",
                story: "一高発表会2019",
                image: "mesh.jpeg",
                icon: "mdi-poll",
                color: "teal darken-1",
            },
        ],
    }),
}
</script>
