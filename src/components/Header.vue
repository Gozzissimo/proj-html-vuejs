<template>
    <header>
        <div class="cont-70">
            <div class="header-top container py-2">
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
            <div class="header-bottom container">
                <nav></nav>
                <div class="jumbotron container"></div>
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
        background-color: #32414e;
        i {
            margin: 0 5px;
        }
        .header-top {
            color: #b3b3b8;
            .social i {
                margin: 0 15px;
            }
        }
    }
</style>
