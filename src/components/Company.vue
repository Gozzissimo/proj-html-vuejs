<template>
    <section>
        <div class="left-side">
        </div>
        <div class="right-side">
        </div>
        <div class="content container">
            <div class="row">
                <div class="col-6">
                    <h3>about the network</h3>
                    <h2>the company</h2>
                    <p>with all of this expertise and capability comes an unrivalled commitment to customer service</p>
                    <div class="row">
                        <div class="col-4 graphic">0%</div>
                        <div class="col-8">
                            <h4>Leadership</h4>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>       
    </section>
</template>

<script>
export default {
    components: "Company",
}
</script>

<style lang="scss" scoped>
    @import "../assets/scss/partials/_variables.scss";

    section {
        position: relative;
        .left-side, .right-side {
            height: 100%;
            width: 50%;
            top: 0;
            position: absolute;
            z-index: -1;
            }
        .left-side {
            background-color: $darkBgColor;
            left: 0;
        }
        .right-side {
            background-image: url('../assets/img/about-5.jpg');
            right: 0;
        }
    }
</style>
