<template>
    <section>
        <div class="container">
            <div class="row line">
                <div class="logo col-2 d-flex">
                    <img src="../assets/img/logo-5.png" alt="less">
                </div>
                <div class="logo col-2 d-flex">
                    <img src="../assets/img/logo-1.png" alt="woo">
                </div>
                <div class="logo col-2 d-flex">
                    <img src="../assets/img/logo-2.png" alt="wordpress">
                </div>
                <div class="logo col-2 d-flex">
                    <img src="../assets/img/logo-3.png" alt="pingdom">
                </div>
                <div class="logo col-2 d-flex">
                    <img src="../assets/img/logo-4.png" alt="jquery">
                </div>
                <div class="logo col-2 d-flex">
                    <img src="../assets/img/logo-5.png" alt="less">
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Customers",
}
</script>

<style lang="scss" scoped>
    @import "../assets/scss/partials/_variables.scss";

    section {
        background-color: $lightBgColor;
        .logo {
            justify-content: center;
            img {
                filter: invert(50%);
                height: 30px;
                object-fit: contain;
            }
        }
    }

</style>
