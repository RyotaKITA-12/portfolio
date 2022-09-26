<template>
    <v-app>
        <v-row align-content="center">
            <div v-for="skill in mainSkills" :key="skill.title">
                <v-col>
                    <v-card elevation="0" class="mt-2 mb-6 mx-1" style="padding: 20px;">
                        <v-row align-content="center">
                            <v-col cols="3">
                                <v-progress-circular :rotate="-90" :size="160" :width="10" :value=skill.value
                                    color="cyan">
                                    <div class="d-flex flex-column black--text ">
                                        <p
                                            class="pb-0 ma-0 text-h7 black--text text-center text--secondary font-weight-bold">
                                            {{ skill.title }}
                                            <br>
                                            {{ skill.subtitle }}
                                        </p>
                                    </div>
                                </v-progress-circular>
                            </v-col>
                            <v-col cols="6">
                                <v-list nav dense disabled>
                                    <v-list-item-group color="primary">
                                        <v-list-item v-for="outline in skill.outlines" :key="outline.title">
                                            <v-list-item-icon>
                                                <v-icon color="cyan lighten-3">{{ outline.icon }}</v-icon>
                                            </v-list-item-icon>
                                            <v-list-item-content>
                                                <v-list-item-title class="cyan--text text--lighten-3">{{ outline.title
                                                }}</v-list-item-title>
                                            </v-list-item-content>
                                        </v-list-item>
                                    </v-list-item-group>
                                </v-list>
                            </v-col>
                            <v-col cols="12">
                                <v-row align-content="center">
                                    <div v-for="item in skill.items" key="item.title">
                                        <v-chip class="ma-2" color="teal" outlined>
                                            <v-icon left>
                                                {{ item.icon }}
                                            </v-icon>
                                            {{ item.title }}
                                        </v-chip>
                                    </div>
                                </v-row>
                            </v-col>
                        </v-row>
                    </v-card>
                </v-col>
            </div>
        </v-row>
    </v-app>
</template>

<script>
export default {
    data: () => ({
        mainSkills: [
            {
                title: "Python",
                value: 100,
                outlines: [
                    {
                        title: "Server Side",
                        icon: "mdi-server",
                    },
                    {
                        title: "Web Scraping",
                        icon: "mdi-server",
                    },
                    {
                        title: "Data Analysis",
                        icon: "mdi-chart-bar",
                    },
                    {
                        title: "Machine Learning / DeepLearning",
                        icon: "mdi-brain",
                    },
                    {
                        title: "Natural Language Processing",
                        icon: "mdi-text-box-outline",
                    },
                    {
                        title: "Image Processing",
                        icon: "mdi-image",
                    },
                    {
                        title: "Audio Processing",
                        icon: "mdi-music",
                    },
                ],
                items: [
                    {
                        title: "fastapi",
                        icon: "mdi-server",
                    },
                    {
                        title: "flask",
                        icon: "mdi-server",
                    },
                    {
                        title: "django",
                        icon: "mdi-server",
                    },
                    {
                        title: "streamlit",
                        icon: "mdi-server",
                    },
                    {
                        title: "beautifulsoup",
                        icon: "mdi-web",
                    },
                    {
                        title: "requests",
                        icon: "mdi-web",
                    },
                    {
                        title: "selenium",
                        icon: "mdi-web",
                    },
                    {
                        title: "numpy",
                        icon: "mdi-chart-bar",
                    },
                    {
                        title: "pandas",
                        icon: "mdi-chart-bar",
                    },
                    {
                        title: "scipy",
                        icon: "mdi-chart-bar",
                    },
                    {
                        title: "sympy",
                        icon: "mdi-chart-bar",
                    },
                    {
                        title: "matplotlib",
                        icon: "mdi-chart-bar",
                    },
                    {
                        title: "seaborn",
                        icon: "mdi-chart-bar",
                    },
                    {
                        title: "networkx",
                        icon: "mdi-chart-bar",
                    },
                    {
                        title: "scikit-learn",
                        icon: "mdi-brain",
                    },
                    {
                        title: "tensorflow",
                        icon: "mdi-brain",
                    },
                    {
                        title: "keras",
                        icon: "mdi-brain",
                    },
                    {
                        title: "pytorch",
                        icon: "mdi-brain",
                    },
                    {
                        title: "onnx",
                        icon: "mdi-brain",
                    },
                    {
                        title: "transformers",
                        icon: "mdi-brain",
                    },
                    {
                        title: "mediapipe",
                        icon: "mdi-brain",
                    },
                    {
                        title: "mecab",
                        icon: "mdi-text-box-outline",
                    },
                    {
                        title: "janome",
                        icon: "mdi-text-box-outline",
                    },
                    {
                        title: "chasen",
                        icon: "mdi-text-box-outline",
                    },
                    {
                        title: "ginza",
                        icon: "mdi-text-box-outline",
                    },
                    {
                        title: "oseti",
                        icon: "mdi-text-box-outline",
                    },
                    {
                        title: "gensim",
                        icon: "mdi-text-box-outline",
                    },
                    {
                        title: "opencv",
                        icon: "mdi-image",
                    },
                    {
                        title: "pillow",
                        icon: "mdi-image",
                    },
                    {
                        title: "scikit-image",
                        icon: "mdi-image",
                    },
                    {
                        title: "pydub",
                        icon: "mdi-music",
                    },
                    {
                        title: "librosa",
                        icon: "mdi-music",
                    },
                ],
            },
            {
                title: "Go",
                value: 75,
                outlines: [
                    {
                        title: "Server Side",
                        icon: "mdi-server",
                    },
                    {
                        title: "Data Analysis",
                        icon: "mdi-chart-bar",
                    },
                    {
                        title: "Machine Learning / DeepLearning",
                        icon: "mdi-brain",
                    },
                    {
                        title: "Natural Language Processing",
                        icon: "mdi-text-box-outline",
                    },
                    {
                        title: "Image Processing",
                        icon: "mdi-image",
                    },
                ],
                items: [
                    {
                        title: "net/http",
                        icon: "mdi-server",
                    },
                    {
                        title: "gin",
                        icon: "mdi-server",
                    },
                    {
                        title: "fiber",
                        icon: "mdi-server",
                    },
                    {
                        title: "beego",
                        icon: "mdi-server",
                    },
                    {
                        title: "kagome",
                        icon: "mdi-text-box-outline",
                    },
                ]
            },
            {
                title: "JavaScript",
                value: 55,
                outlines: [
                    {
                        title: "Client Side",
                        icon: "mdi-application-brackets-outline",
                    },
                    {
                        title: "Google App Script",
                        icon: "mdi-google",
                    },
                ],
                items: [
                    {
                        title: "nuxt.js",
                        icon: "mdi-server",
                    },
                    {
                        title: "vue.js",
                        icon: "mdi-application-brackets-outline",
                    },
                    {
                        title: "vuetify",
                        icon: "mdi-application-brackets-outline",
                    },
                    {
                        title: "react.js",
                        icon: "mdi-application-brackets-outline",
                    },
                    {
                        title: "material-ui",
                        icon: "mdi-application-brackets-outline",
                    },
                    {
                        title: "google-apps-script",
                        icon: "mdi-google",
                    },
                ]
            },
            {
                title: "C",
                value: 35,
            },
            {
                title: "Swift",
                value: 25,
                items: [
                    {
                        title: "swift-ui",
                        icon: "mdi-apple",
                    },
                ]
            },
            {
                title: "C#",
                value: 25,
                items: [
                    {
                        title: "unity",
                        icon: "mdi-unity",
                    },
                ]
            },
            {
                title: "Vim",
                value: 100,
                items: [
                    {
                        title: "vim-script",
                        icon: "mdi-pencil",
                    },
                ]
            },
            {
                title: "Database",
                value: 100,
                items: [
                    {
                        title: "postgresql",
                        icon: "mdi-database-search",
                    },
                    {
                        title: "mysql",
                        icon: "mdi-database-search",
                    },
                    {
                        title: "sqlite",
                        icon: "mdi-database-search",
                    },
                ]
            },
            {
                title: "Shell",
                value: 50,
                items: [
                    {
                        title: "zsh",
                        icon: "mdi-laptop",
                    },
                    {
                        title: "bash",
                        icon: "mdi-laptop",
                    },
                ]
            },
            {
                title: 'Linux',
                value: 50,
                items: [
                    {
                        title: "arch-linux",
                        icon: "mdi-laptop",
                    },
                    {
                        title: "fedora",
                        icon: "mdi-laptop",
                    },
                    {
                        title: "elementary-os",
                        icon: "mdi-laptop",
                    },
                ]
            },
            {
                title: 'Git',
                subtitle: 'GitHub',
                value: 75,
            },
            {
                title: 'Docker',
                subtitle: 'Docker Compose',
                value: 75,
            },
        ]
    }),
}
</script>

