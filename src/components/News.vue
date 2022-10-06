<template>
    <v-app>
        <v-timeline v-for="item in items" :key="item.text" align-top dense>
            <v-timeline-item color="teal lighten-3" small>
                <v-row class="pt-1">
                    <v-col cols="3">
                        <p class="indigo--text text--lighten-4"><strong>{{ item.time }}</strong></p>
                    </v-col>
                    <v-col>
                        <a :href="item.link">
                            <p class="light-blue--text text--lighten-3"><strong>{{ item.text }}</strong></p>
                        </a>
                    </v-col>
                </v-row>
            </v-timeline-item>
        </v-timeline>
    </v-app>
</template>
<script>
export default {
    data: () => ({
        items: [
            {
                time: "2022-08-29",
                text: "データサイエンス学部生がオンラインハッカソンにて優秀賞を受賞",
                link: "https://www.musashino-u.ac.jp/news/20220829-02.html",
            },
            {
                time: "2022-06-22",
                text: "データサイエンス学部３年生がオンラインハッカソンにて努力賞を受賞",
                link: "https://www.musashino-u.ac.jp/news/20220622-02.html",
            },
            {
                time: "2022-03-30",
                text: "【武蔵野大学】ヤフー主催の学生ハッカソンイベントにてデータサイエンス学部生が優秀賞を受賞！ - PRTIMES",
                link: "https://prtimes.jp/main/html/rd/p/000000090.000067788.html",
            },
            {
                time: "2022-03-24",
                text: "【武蔵野大学】データサイエンス学部１・３年生３名が「情報処理学会 第84回全国大会」で「学生奨励賞」を受賞 - PRTIMES",
                link: "https://prtimes.jp/main/html/rd/p/000000087.000067788.html",
            },
            {
                time: "2021-10-01",
                text: "【武蔵野大学】学生対象のアプリ開発イベント『技育CAMP』にてデータサイエンス学部生の３チームが「努力賞」を受賞 - PRTIMES",
                link: "https://prtimes.jp/main/html/rd/p/000000062.000067788.html",
            },
            {
                time: "2021-09-24",
                text: "【武蔵野大学】今夏開催のアプリ開発イベントにてデータサイエンス学部生が優勝！ - PRTIMES",
                link: "https://prtimes.jp/main/html/rd/p/000000060.000067788.html",
            },
            {
                time: "2020-02-14",
                text: "愛知県高等学校職業教育技術認定事業グランプリ受賞",
                link: "https://www.chubu-ichi.ed.jp/main/news/6802/",
            },
        ]
    }),
}
</script>
<style>
a {
    text-decoration: none;
}
</style>
