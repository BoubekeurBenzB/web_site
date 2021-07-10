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
                <img src="@/assets/photo_identite_bob.jpg" alt="img_profile" />
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "About",
    props: {
        title: String,
        text: String,
        citation: String,
        location: String,
    },
};
</script>

<style lang="scss" scoped>
.about {
    margin: 0 5rem;
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
}

.text,
.img {
    width: 47%;
    padding: 3rem 1rem;
}

.text h1 {
    color: #4c5d6a;
    font-size: 40px;
    margin-bottom: 2rem;
}
.text p {
    color: #88888c;
    margin-bottom: 1rem;
    font-size: 20px;
    white-space: pre-line;
}

.content-2 {
    text-align: center;
}
.img h2 {
    color: #4c5d6a;
    font-size: 35px;
    margin-bottom: 5rem;
}
.img img {
    height: 300px;
    width: 300px;
    border-radius: 50%;
    object-fit: cover;
}

/** responsive */

/** tablet & ipad */
@media screen and (min-width: 768px) and (max-width: 1024px) {
    .text,
    .img {
        padding: 3rem 0;
    }

    .text h1 {
        font-size: 30px;
    }
    .text p {
        font-size: 18px;
    }

    .img h2 {
        font-size: 25px;
    }
    .img img {
        height: 250px;
        width: 250px;
    }
}

/** mobile */
@media screen and (max-width: 768px) {
    .about {
        margin: 0 1rem;
        flex-direction: column;
    }

    .text,
    .img {
        width: 100%;
        padding: 3rem 1rem;
    }

    .text h1 {
        font-size: 50px;
    }
    .text p {
        font-size: 25px;
    }

    .img h2 {
        font-size: 40px;
    }
    .img img {
        height: 350px;
        width: 350px;
    }
}
</style>
