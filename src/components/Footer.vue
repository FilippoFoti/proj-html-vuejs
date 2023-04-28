<script>
export default {
    name: "Footer"
}
</script>

<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col">
                    <h3>SEND A MESSAGE</h3>
                    <h2>Get in <span>Touch</span></h2>
                    <p>We will respond to your message as soon as possible.</p>
                    <form action="">
                        <input type="text" placeholder="Name">
                        <input type="email" placeholder="Email">
                        <input type="text" placeholder="Phone">
                        <select name="" id="">
                            <option value="">More Info</option>
                            <option value="">Paese</option>
                            <option value="">Citta</option>
                            <option value="">Via</option>
                        </select>
                        <textarea rows="5" cols="1" placeholder="Message"></textarea>
                    </form>
                    <button>SEND</button>
                </div>
                <div class="col map">
                    <h4>Example Inc.</h4>
                    <p>Lorem ipsum dolor sit amer, consectetur adipiscingelit.</p>
                    <p>Praesent diam lacus, dapibus sed imperdiet consectetur.</p>
                    <ul>
                        <li>
                            <div class="circle">
                                <i class="fa-solid fa-phone"></i>
                            </div>
                            <span>+1 (305) 1234-5678</span>
                        </li>
                        <li>
                            <div class="circle">
                                <i class="fa-solid fa-envelope"></i>
                            </div>
                            <span>hello@example.com</span>
                        </li>
                        <li>
                            <div class="circle">
                                <i class="fa-solid fa-location-dot"></i>
                            </div>
                            <span>Main Avenue, 987</span>
                        </li>
                    </ul>
                    <button>VIEW MAP</button>
                </div>
            </div>
        </div>
    </footer>
    <div class="footer-bottom">
        <div class="container">
            <div class="left">
                <p>Enjoy the low price. We are tracking any intention of piracy.</p>
            </div>
            <div class="right">
                <p>© 2020 NEXGEN is Proudly Powered by <span class="green">Codings</span>.</p>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

footer {
    background-color: rgba(17, 17, 23, 1);
    color: white;

    .container {
        width: 60%;
        margin: 0 auto;
        padding: 100px 0;

        .row {
            display: flex;
            gap: 40px;

            .col {
                width: calc(100% / 3 * 2);

                h3 {
                    color: rgba(0, 165, 165, 1);
                    font-size: 0.9rem;
                    padding-bottom: 20px;
                }

                h2 {
                    font-size: 2.3rem;
                    color: white;
                    padding-bottom: 20px;

                    span {
                        background-color: rgba(14, 39, 45, 1);
                        padding: 0 10px;
                        border-radius: 3px;
                        color: white;
                    }
                }

                p {
                    font-size: 0.8rem;
                    color: #e4eae6;
                    padding-bottom: 40px;
                }

                form {
                    display: flex;
                    flex-wrap: wrap;
                    gap: 10px;
                    padding-bottom: 20px;

                    input {
                        width: calc(50% - 5px);
                        font-size: 1rem;
                        outline: 0;
                        padding: 10px;
                        background-color: rgba(29, 29, 35, 1);
                        color: #e4eae6;
                        border-radius: 5px;
                        border: 0;
                    }

                    select {
                        width: calc(50% - 5px);
                        font-size: 1rem;
                        outline: 0;
                        padding: 10px 6.5px;
                        background-color: rgba(29, 29, 35, 1);
                        color: #e4eae6;
                        border-radius: 5px;
                        border: 0;
                    }

                    textarea {
                        width: 100%;
                        font-size: 1rem;
                        outline: 0;
                        padding: 10px;
                        background-color: rgba(29, 29, 35, 1);
                        color: #e4eae6;
                        border-radius: 5px;
                        border: 0;
                        font-family: 'Poppins', sans-serif;
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
            }

            .map {
                width: calc(100% / 3);

                h4 {
                    font-size: 1.5rem;
                    padding-bottom: 10px;
                }

                p {
                    padding-bottom: 10px;
                }

                ul {
                    list-style-type: none;
                    padding: 20px 0 15px 0;


                    li {
                        display: flex;
                        align-items: center;
                        gap: 10px;
                        padding-bottom: 15px;

                        .circle {
                            width: 35px;
                            height: 35px;
                            border-radius: 50%;
                            background-color: rgba(15, 33, 40, 1);
                            display: flex;
                            align-items: center;
                            justify-content: center;
                            cursor: pointer;

                            &:hover {
                                transform: scale(1.5);
                                transition: 0.3s;
                            }

                            i {
                                color: rgba(5, 130, 131, 1);
                            }
                        }

                        span {
                            font-size: 0.9rem;
                            color: rgba(5, 130, 131, 1);
                        }
                    }
                }

                button {
                    padding: 10px 20px;
                    border-radius: 5px;
                    border: 1px solid rgba(5, 130, 131, 1);
                    color: white;
                    font-weight: bold;
                    background-color: transparent;
                    cursor: pointer;

                }
            }
        }
    }
}

.footer-bottom {
    background-color: rgba(13, 13, 17, 1);
    height: 60px;

    .container {
        height: 100%;
        width: 60%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .left,
        .right {
            color: #e4eae6;
            font-size: 0.75rem;

            span {
                color: rgba(5, 130, 131, 1);
            }
        }
        
    }
}
</style>