<script>
import Card from './Card.vue';


export default {
    name: "SectionFive",
    components: {
        Card
    },
    props: {
        arrayThree: Array
    }
}
</script>

<template>
    <main>
        <div class="container">
            <h3>CUSTOMER TESTIMONIALS</h3>
            <h2>Trusted <span>Feedback</span></h2>
            <p>We work intensively in search of ideals that can add up in the lives of our customers. This is what moves us
                and we are grateful for the recognition.</p>
            <Card :arrayThree="arrayThree" />
        </div>
    </main>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

main {
    background-color: rgba(238, 244, 237, 1);

    .container {
        width: 60%;
        margin: 0 auto;
        padding: 100px 0;
        text-align: center;

        h3 {
            color: rgba(0, 165, 165, 1);
            font-size: 0.9rem;
            padding-bottom: 20px;
        }

        h2 {
            font-size: 2.3rem;
            color: black;
            padding-bottom: 20px;

            span {
                background-color: rgba(218, 236, 237, 1);
                padding: 0 10px;
                border-radius: 3px;
                color: rgba(0, 165, 165, 1);
            }
        }

        p {
            width: 70%;
            margin: 0 auto;
            font-size: 0.8rem;
            padding-bottom: 30px;
        }
    }
}
</style>