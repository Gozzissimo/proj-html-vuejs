<template>
    <header>
        <div class="header-top">
            <div class="header-top container py-2 cont-70">
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
            <div class="header-bottom container cont-70">
                <nav>
                    <img src="" alt="">
                </nav>
                <div class="jumbotron row"></div>
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
    header {
        i {
            margin: 0 5px;
        }
        .header-top {
            background-color: #32414e;
            color: #b3b3b8;
            .social i {
                margin: 0 15px;
            }
        }
        .header-bottom {
            background-image: url('../assets/img/jumbo.jpg');
        }
    }
</style>
