<script>

export default {
    name: "Headertop"
}
</script>

<template>
    <div class="header">
        <div class="top">
            <div class="left">
                <ul>
                    <li>
                        <i class="fa-solid fa-clock"></i>
                        <span>Open Hours: Mon - Sat - 9:00 - 18-00</span>
                    </li>
                </ul>
            </div>
            <div class="right">
                <ul>
                    <li>
                        <i class="fa-solid fa-phone"></i>
                        <span>+1 (305) 1234-5678</span>
                    </li>
                    <li>
                        <i class="fa-solid fa-envelope"></i>
                        <span>hello@example.com</span>
                    </li>
                    <li>
                        <i class="fa-brands fa-facebook-f"></i>
                    </li>
                    <li>
                        <i class="fa-brands fa-twitter"></i>
                    </li>
                    <li>
                        <i class="fa-brands fa-linkedin-in"></i>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

.header {
    height: 35px;
    background-color: rgba(33, 51, 62, 1);
    display: flex;
    align-items: center;
    font-size: 0.7rem;
    color: rgba(192, 195, 208, 1);

    .top {
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 60%;
        margin: 0 auto;

        ul {
            display: flex;
            list-style-type: none;
            gap: 25px;

            span {
                margin-left: 5px;
            }
        }
    }
}
</style>