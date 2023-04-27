<script>

export default {
    name: "SectionTwo",
}
</script>

<template>
    <main>
        <div class="container">
            <div class="left">
                <h3>ABOUT THE NETWORK</h3>
                <h2><span>The</span> Company</h2>
                <p>Lorem Ipsum dolor sit amet, consectetur adipiscing elit. Cras iaculis diam varius diam ultricies Iacinia.
                </p>
                <div class="row">
                    <div class="col">
                        <h2>0</h2>
                        <h3>Employees</h3>
                        <p>Lorem ipsum dolor sit amet.</p>
                    </div>
                    <div class="col">
                        <h2>0</h2>
                        <h3>Partners</h3>
                        <p>Lorem ipsum dolor sit amet.</p>
                    </div>
                    <div class="col">
                        <h2>0</h2>
                        <h3>Customers</h3>
                        <p>Lorem ipsum dolor sit amet.</p>
                    </div>
                </div>
                <button>GET IN TOUCH</button>
                <button class="color">READ MORE</button>
            </div>
            <div class="right"></div>
        </div>
        <div class="pattern"></div>
    </main>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

main {
    // height: 500px;
    position: relative;


    .container {
        // width: 60%;
        // margin: 0 auto;
        height: 100%;
        display: flex;

        .left {
            width: 30%;
            margin-left: 20%;
            padding: 100px 0;

            h3 {
                padding: 20px 0;
                color: rgba(0, 165, 165, 1);
                font-size: 0.9rem;
            }

            h2 {
                font-size: 2.3rem;

                span {
                    color: rgba(5, 130, 131, 1);
                    background-color: rgba(218, 236, 237, 1);
                    padding: 0 10px;
                    border-radius: 3px;
                }
            }

            p {
                font-size: 0.85rem;
                padding: 20px 0 40px 0;
            }

            .row {
                display: flex;
                gap: 20px;

                .col {
                    width: calc(100% / 3 - 20px);

                    h2 {
                        padding-left: 20px;
                        color: rgba(5, 130, 131, 1);
                    }

                    h3 {
                        padding: 0;
                        color: black;
                        font-size: 1.2rem;
                    }
                }
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
                color: rgba(5, 130, 131, 1);
                margin-left: 25px;
            }
        }

        .right {
            width: 50%;
            background-image: url(../assets/img/about-5.jpg);
            background-position: center;
            background-size: cover;
        }
    }

    .pattern {
        width: 170px;
        height: 75px;
        background: radial-gradient(circle, #7ED5D5 25%, transparent 26%);
        background-size: 1.2em 1.2em;
        background-color: transparent;
        opacity: 0.6;
        position: absolute;
        left: 50%;
        bottom: -36px;
        transform: translate(-50%)
    }
}
</style>