<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="left-side col-5 offset-1">
                    <h3>newsletter</h3>
                    <h2 class="my-3"><span class="green-bg">know</span> first</h2>
                    <p>Follow closely and receive content about our company and the news of the current market</p>
                </div>
                <div class="right-side col-5 row">
                    <form action="#">
                        <input class="col-12" placeholder="Name" type="text" name="news-name" id="news-name">
                        <input class="col-12" placeholder="Email" type="email" name="news-email" id="news-email">
                        <input class="green-button" type="submit" value="subscribe">
                    </form>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Newsletter",
}
</script>

<style lang="scss" scoped>
    @import "../assets/scss/partials/_variables.scss";

    section {
        background-image: url('../assets/img/bg-1.jpg');
        background-position: center;
        background-size: cover;
        .left-side {
            h2 {
                color: $whiteFontColor;
            }
        }
        .right-side input {
            margin-bottom: 1em;
        }
    }
</style>