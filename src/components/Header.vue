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
                        <i class="fab fa-facebook-f"></i>
                        <i class="fab fa-twitter"></i>
                        <i class="fab fa-linkedin-in"></i>
                    </div>
                </div>
            </div>
        </div>
        <div class="header-bottom">
            <div class="background-opacity py-2">
                <div class="container cont-70">
                    <nav class="row">
                        <div class="col-4">
                            <a class="logo-img" href=""><img src="../assets/img/logo.svg" alt=""></a>
                        </div>
                        <div class="col-8 text-end">
                            <ul class="list-inline">
                                <li><a href="#">home</a></li>
                                <li><a href="#">services</a></li>
                                <li><a href="#">skills</a></li>
                                <li><a href="#">partners</a></li>
                                <li><a href="#">blog</a></li>
                                <li><a href="#"><button type="button" class="green-button">get in touch</button></a></li>
                            </ul>
                        </div>
                    </nav>
                    <div class="jumbotron row">
                        <div></div>
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
        i {
            margin: 0 5px;
        }
        .header-top {
            background-color: #4d5a65;
            color: #e5ebe5;
            .social i {
                margin: 0 15px;
            }
        }
        .header-bottom {
            background-image: url('../assets/img/jumbo.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            height: 500px;
            .background-opacity {
                background-color: #1211178a;
                height: 500px;
                a {
                    text-decoration: none;
                    display: block;
                    text-transform: uppercase;
                    color: #e5ebe5;
                    margin: 0 10px;
                    line-height: 3em;
                }
                button {
                    text-transform: uppercase;
                }
                .logo-img {
                    width: 150px;
                    img {
                        width: 100%;
                    }
                }
            }
        }
    }
</style>
