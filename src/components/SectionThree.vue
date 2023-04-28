<script>
import Nav from './Nav.vue';

export default {
    name: "SectionThree",
    components: {
        Nav
    },
    props: {
        arrayTwo: Array
    }
}
</script>

<template>
    <main>
        <div class="container">
            <h3>WE DO MORE FOR EVERYONE</h3>
            <h2>Actions & <span>Projects</span></h2>
            <Nav :arrayTwo="arrayTwo" />
            <div class="row">
                <div class="col">
                    <img src="../assets/img/project-1.jpg" alt="">
                    <h4>Academic professional program in social media</h4>
                </div>
                <div class="col">
                    <img src="../assets/img/project-2.jpg" alt="">
                    <h4>President's speech at the annual meeting</h4>
                </div>
                <div class="col">
                    <img src="../assets/img/project-3.jpg" alt="">
                    <h4>International business trip in Shanghai</h4>
                </div>
                <div class="col">
                    <img src="../assets/img/project-4.jpg" alt="">
                    <h4>Technology workshop whit education theme</h4>
                </div>
                <div class="col">
                    <img src="../assets/img/project-5.jpg" alt="">
                    <h4>Donation of clothes and food to the partner NGO</h4>
                </div>
                <div class="col">
                    <img src="../assets/img/project-6.jpg" alt="">
                    <h4>Confraternization of the procurement team</h4>
                </div>
            </div>
        </div>
    </main>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

main {
    background-color: rgba(17, 17, 23, 1);

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
            color: white;
            padding-bottom: 30px;

            span {
                background-color: rgba(14, 39, 45, 1);
                padding: 0 10px;
                border-radius: 3px;
            }
        }

        .row {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            padding-top: 20px;


            .col {
                width: calc(100% / 3 - 14px);
                position: relative;

                img {
                    border-radius: 10px;
                    background-color: black;
                    opacity: 0.5;

                    &:hover {
                        opacity: 1;
                    }
                }

                h4 {
                    color: white;
                    position: absolute;
                    bottom: 45px;
                    left: 50%;
                    transform: translate(-50%);
                    font-size: 1.2rem;
                    width: 90%;

                }
            }
        }
    }
}
</style>