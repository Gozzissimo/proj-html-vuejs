<template>
    <header>
        <div class="header-top">
            <div class="container py-2 cont-70">
                <div class="row">
                    <div class="col-6">
                        <i class="fas fa-clock"></i>
                        Open Hours: Mon - Sat - 9:00 - 18:00
                    </div>
                    <div class="col-2 text-end">
                        <i class="fas fa-phone-alt"></i>
                        +1 (305) 1234-5678
                    </div>
                    <div class="col-2 text-end">
                        <i class="fas fa-envelope"></i>
                        hello@example.com
                    </div>
                    <div class="col-2 text-end social">
                        <a href="#">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="#">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="#">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
        <div class="header-bottom">
            <div class="background-opacity py-2">
                <div class="container">
                    <nav class="row">
                        <div class="col-2">
                            <a class="logo-img" href=""><img src="../assets/img/logo.svg" alt="logo"></a>
                        </div>
                        <div class="col-10 text-end">
                            <ul class="list-inline">
                                <li><a href="#">home</a></li>
                                <li><a href="#">services</a></li>
                                <li><a href="#">skills</a></li>
                                <li><a href="#">partners</a></li>
                                <li><a href="#">blog</a></li>
                                <li><a href="#contact"><button type="button" class="green-button">get in touch</button></a></li>
                            </ul>
                        </div>
                    </nav>
                    <div class="jumbotron row">
                        <div class="col-3 offset-7">
                            <h1 class="jumbo-title">
                                <span class="highlight">Logistics</span>
                                that goes further.
                            </h1>
                            <p class="jumbo-desc">
                                For 20 years working with the most innovative in the field of transport
                            </p>
                            <div class="jumbo-buttons d-flex">
                                <a href="#contact"><button class="green-button">get in touch</button></a>
                                <a href=""><button class="borderless-button">read more</button></a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
}
</script>

<style lang="scss" scoped>
    @import "../assets/scss/partials/_variables.scss";

    header {
        a {
            color: $whiteFontColor;
        }
        i {
            margin: 0 5px;
        }
        .header-top {
            background-color: $darkGreyBgColor;
            color: $whiteFontColor;
            font-size: 0.9em;
            .social i {
                margin: 0 15px;
            }
        }
        .header-bottom {
            background-image: url('../assets/img/jumbo.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            background-position: left;
            height: 600px;
            .background-opacity {
                background-color: #12111786;
                height: 600px;
                nav {
                    li a {
                        text-decoration: none;
                        display: block;
                        text-transform: uppercase;
                        color: $whiteFontColor;
                        line-height: 3em;
                        margin: 0 20px;
                    }
                    button {
                        text-transform: uppercase;
                    }
                    .logo-img {
                        width: 150px;
                        img {
                            width: 70%;
                        }
                    }
                }
                .jumbotron {
                    margin-top: 3em;
                    .jumbo-title {
                        font-weight: 800;
                        font-size: 3.5em;
                        color: $whiteFontColor;
                        .highlight {
                            background: linear-gradient( rgba(255, 255, 255, 0) 40%, $greenFontColor 100%);
                        }
                    }
                    .jumbo-desc {
                        color: $greyFontColor;
                        margin: 20px 0;
                        font-size: 1.2em;
                    }
                    .jumbo-buttons {
                        a {
                            margin-right: 20px;
                        }
                    }
                }    
            }
        }
    }
</style>
