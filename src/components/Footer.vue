<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="row">
                    <div class="col-3 box d-flex me-3">
                        <img src="../assets/img/logo.svg" alt="logo">
                        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
                        <ul>
                            <li>
                                <i class="fas fa-phone-alt"></i>+1 (305) 1234-5678
                            </li>
                            <li>
                                <i class="fas fa-envelope"></i>hello@example.com
                            </li>
                            <li>
                                <i class="fas fa-map-marker-alt"></i>Main Avenue, 987
                            </li>
                        </ul>
                        <a href="#contact">
                            <button class="borderless-button">get in touch</button>
                        </a>
                    </div>
                    <div class="col-3 me-3 box">
                        <h4>About</h4>
                        <ul>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>the company</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>institutional</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>social & events</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>innovation</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>environment</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>technology</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col-3 me-3 box">
                        <h4>Transport</h4>
                        <ul>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>industrialized</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>chemicals</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>packaged liquids</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>construction</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>laminated woods</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>and others</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col-3 box">
                        <h4>Support</h4>
                        <ul>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>responsibility</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>terms of use</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>about cookies</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>privacy policy</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>accessibility</a>
                            </li>
                            <li>
                                <a href="#"><i class="fas fa-chevron-right"></i>information</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-bottom">

        </div>
    </footer>
</template>

<script>
export default {
    name: "Footer",
}
</script>

<style lang="scss" scoped>
    @import "../assets/scss/partials/_variables.scss";

    .footer-top {
        background-image: url('../assets/img/bg-10.jpg');
        background-position: center;
        background-size: cover;
        padding: 8em;
        color: $greyFontColor;
        .box {
            width: calc((100% / 4) - 0.8em);
            &:not(:first-child) {
                background-color: rgba($greyFontColor, 0.1);
                border-radius: 10px;
                padding: 3em;
            }
            &:first-child {
                flex-direction: column;
                justify-content: space-between;
            }
            img {
                width: 50%;
            }
            h4 {
                color: $whiteFontColor;
            }
            ul {
                padding: 0;
                li {
                    margin-bottom: 0.5em;
                    i {
                        margin-right: 0.5em;
                    }
                    a {
                        text-transform: capitalize;
                    text-decoration: none;
                    color: $greyFontColor;
                    }
                }
            }
        }
    }
</style>