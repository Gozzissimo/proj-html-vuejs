<template>
    <section>
        <div class="left-side">
        </div>
        <div class="right-side">
            <img src="../assets/img/about-5.jpg" alt="skyscrapers">
        </div>
        <div class="container">
            <div class="row">
                <div class="content col-6">
                    <div class="mb-5">
                        <h3>about the network</h3>
                        <h2><span class="text-center">the</span> company</h2>
                        <p>with all of this expertise and capability comes an unrivalled commitment to customer service</p>
                    </div>
                    <div class="stats row">
                        <div class="col-4 graphic">0<span>%</span></div>
                        <div class="col-8">
                            <h4>Leadership</h4>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        </div>
                    </div>
                    <div class="stats row">
                        <div class="col-4 graphic">0<span>%</span></div>
                        <div class="col-8">
                            <h4>Pscyhology</h4>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        </div>
                    </div>
                    <div class="stats row">
                        <div class="col-4 graphic">1<span>%</span></div>
                        <div class="col-8">
                            <h4>flexibility</h4>
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
            right: 0;
            img {
                object-fit: cover;
                height: 100%;
                width: 100%;
            }
        }
        .content {
            padding-right: 4em;
            h2, h4 {
                color: $whiteFontColor;
            }
            h2 {
                margin-top: 20px;
                span {
                    background-color: rgba($greenFontColor, 0.1);
                    display: inline-block;
                    height: 1.2em;
                    width: 2.3em;
                    line-height: 1.2em;
                }
            }
            .stats {
                margin-bottom: 2em;
                .graphic {
                    background-color: $darkBgColor;
                    border-radius: 100%;
                    border: 10px solid rgba($darkGreyBgColor, 0.1);
                    width: 100px;
                    height: 100px;
                    line-height: 75px;
                    margin-right: 1em;
                    text-align: center;
                    font-weight: bold;
                    font-size: 2em;
                    color: $greyFontColor;
                    span {
                        font-size: 0.5em;
                    }
                }
            }
        }
    }
</style>
