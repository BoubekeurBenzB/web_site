<template>
    <section class="skills">
        <div class="text">
            <h1>{{ title }}</h1>
            <p>{{ text }}</p>
        </div>
        <div class="langagues">
            <div class="language" v-for="lang in languages" :key="lang.id">
                <h1>{{ lang.langague }}</h1>
                <h3>{{ lang.type }}</h3>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Skills",
    data() {
        return {
            languages: [
                {
                    langague: "HTML",
                    type: "HTML5",
                },
                {
                    langague: "CSS",
                    type: "CSS3",
                },
                {
                    langague: "JavaScript",
                    type: "JavaScript",
                },
                {
                    langague: "JavaScript",
                    type: "VueJS",
                },
            ],
        };
    },
    props: {
        title: String,
        text: String,
    },
};
</script>

<style lang="scss" scoped></style>
