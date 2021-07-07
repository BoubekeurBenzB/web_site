<template>
    <section class="about">
        <div class="text">
            <div class="content">
                <h1>{{ title }}</h1>
                <p>{{ text }}</p>
                <p>{{ citation }}</p>
            </div>
        </div>
        <div class="img">
            <div class="content-2">
                <h2>{{ location }}</h2>
                <img src="@/assets/photo_identite_bob.jpg" alt="img_profile">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'About',
    props: {
        title: String,
        text: String,
        citation: String,
        location: String
    }
}
</script>

<style lang="scss" scoped>
</style>