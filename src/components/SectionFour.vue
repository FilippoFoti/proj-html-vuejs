<script>
export default {
    name: "SectionFour"
}
</script>

<template>
    <main>
        <div class="container">
            <h3>HOW IT WORKSIN PRACTICE</h3>
            <h2><span>Process</span> Management</h2>
            <p>We work whit innovative methodologies to ensure that the entire reformatting process is done from start to
                finischas planned.</p>
            <div class="row">
                <div class="col">
                    <h5><span>01</span></h5>
                    <h4>Collection of information</h4>
                    <p>Lorem ipsum dolor sit emet consectetur.</p>
                </div>
                <div class="col">
                    <h5><span>02</span></h5>
                    <h4>Strategic planning</h4>
                    <p>Lorem ipsum dolor sit emet consectetur.</p>
                </div>
                <div class="col">
                    <h5><span>03</span></h5>
                    <h4>Assignment of responsibilities</h4>
                    <p>Lorem ipsum dolor sit emet consectetur.</p>
                </div>
                <div class="col">
                    <h5><span>04</span></h5>
                    <h4>Formattin process</h4>
                    <p>Lorem ipsum dolor sit emet consectetur.</p>
                </div>
                <div class="col">
                    <h5><span>05</span></h5>
                    <h4>Continuity formalization</h4>
                    <p>Lorem ipsum dolor sit emet consectetur.</p>
                </div>
            </div>
        </div>
        <div class="border"></div>
    </main>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

main {
    position: relative;

    .container {
        width: 80%;
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
            width: 50%;
            margin: 0 auto;
            font-size: 0.8rem;
        }

        .row {
            display: flex;
            padding-top: 30px;

            .col {
                width: calc(100% / 5);
                h5 {
                    margin: 0 auto;
                    height: 30px;
                    width: 30px;
                    border-radius: 50%;
                    background-color: rgba(218, 236, 237, 1);
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    margin-bottom: 15px;
                    position: relative;
                    z-index: 1;

                    span {
                        color: rgba(0, 165, 165, 1);
                        font-size: 0.9rem;
                    }
                }

                h4 {
                    padding-bottom: 15px;
                    font-size: 1.3rem;
                }

                p {
                    width: 100%;
                }
            }
        }
    }

    .border {
        border: 3px solid rgba(218, 236, 237, 1);
        width: 100%;
        position: absolute;
        top: 300px;
        left: 0;
    }
}
</style>