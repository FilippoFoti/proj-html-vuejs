<script>
import Nav from './Nav.vue';

export default {
    name: "HeaderBottom",
    components: {
        Nav
    },
    props: {
        menu: Array
    },
}

</script>

<template>
    <div class="header">
        <div class="bottom">
            <div class="menu">
                <div class="logo">
                    <h2 class="green">NEX</h2>
                    <h2>GEN</h2>
                </div>
                <div class="list">
                    <Nav :menu="menu" />
                    <i class="fa-regular fa-user"></i>
                    <button>GET IN TOUCH</button>
                </div>
            </div>
            <div class="jumbotron">
                <h3>HUMAN RESOURCES</h3>
                <h1>Get More Productivity</h1>
                <div class="backgroud"></div>
                <p>Planning, recruitment and seection process and performance evaluation of employees.</p>
                <button>GET IN TOUCH</button>
                <button class="color">READ MORE</button>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

.header {
    background-image: url(../assets/img/bg-4.jpg);
    background-size: cover;
    height: 600px;

    .bottom {
        width: 60%;
        margin: 0 auto;
        padding-top: 20px;

        .menu {
            display: flex;
            align-items: center;
            justify-content: space-between;

            .logo {
                display: flex;
                font-size: 0.7rem;
                color: white;
                letter-spacing: 5px;

                h2 {
                    margin-top: 8px;
                }

                .green {
                    color: rgba(0, 165, 165, 1);
                    background-color: rgba(0, 165, 165, 0.2);
                    border-top-left-radius: 60px;
                    border-bottom-left-radius: 60px;
                    padding: 8px 0 8px 20px;
                    margin: 0;
                }

            }

            .list {
                display: flex;
                align-items: center;
                gap: 25px;
                color: white;

                ul {
                    display: flex;
                    gap: 20px;
                    list-style-type: none;
                }

                button {
                    padding: 10px 20px;
                    border-radius: 5px;
                    border: 0;
                    color: white;
                    font-weight: bold;
                    background-color: rgba(5, 130, 131, 1);
                    cursor: pointer;
                }
            }
        }

        .jumbotron {
            width: 50%;
            margin-top: 120px;


            h3 {
                color: rgba(0, 165, 165, 1);
                font-size: 0.9rem;
            }

            h1 {
                font-size: 4rem;
                color: white;
                z-index: 999;
                position: relative;
                line-height: 65px;
                margin: 15px 0;
            }

            .backgroud {
                width: 403px;
                height: 35px;
                background-color: rgba(5, 130, 131, 0.4);
                border-radius: 3px;
                position: absolute;
                top: 347px;
                left: 308px;
            }

            p {
                color: #e4eae6;
                font-size: 1.1rem;
                margin-bottom: 30px;
            }

            button {
                padding: 10px 20px;
                border-radius: 5px;
                border: 1px solid rgba(5, 130, 131, 1);
                color: white;
                font-weight: bold;
                background-color: rgba(5, 130, 131, 1);
                cursor: pointer;
            }

            .color {
                background-color: transparent;
                margin-left: 25px;
            }
        }
    }
}
</style>