<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="left-side col-6">
                    <h3>our editorial content</h3>
                    <h2 class="my-3">latest <span class="green-bg green">news</span></h2>
                    <p>Every week we publish content about what is best in the business world.</p>
                </div>
                <div class="right-side col-6 d-flex">
                    <button :class="(!isActive ? 'd-block' : 'd-none')" @click="reveal" class="green-button">see all</button>
                    <button :class="(isActive ? 'd-block' : 'd-none')" @click="reveal" class="green-button">see less</button>
                </div>
            </div>
            <div class="row">
                <a class="box col-4 text-center" href="#">
                    <div class="opacity-box">
                        <img src="../assets/img/news-1.jpg" alt="">
                        <h4>
                            Increasing creativity is possible for everyone
                        </h4>
                    </div>
                </a>
                <a class="box col-4 text-center" href="#">
                    <div class="opacity-box">
                        <img src="../assets/img/news-2.jpg" alt="">
                        <h4>
                            Because market reasearch is part of the business plan
                        </h4>
                    </div>
                </a>
                <a class="box col-4 text-center" href="#">
                    <div class="opacity-box">
                        <img src="../assets/img/news-3.jpg" alt="">
                        <h4>
                            Working from home is now a trend
                        </h4>
                    </div>
                </a>
                <a :class="isActive ? 'd-flex' : 'd-none'" class="box col-4 text-center" href="#">
                    <div class="opacity-box">
                        <img src="../assets/img/news-4.jpg" alt="">
                        <h4>
                            Meglio un uovo oggi che una gallina domani
                        </h4>
                    </div>
                </a>
                <a :class="isActive ? 'd-flex' : 'd-none'" class="box col-4 text-center" href="#">
                    <div class="opacity-box">
                        <img src="../assets/img/news-5.jpg" alt="">
                        <h4>
                            Drinking coffee helps a lot
                        </h4>
                    </div>
                </a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "News",

    data() {
        return {
            isActive: false,
        };
    },

    methods: {
        reveal() {
            if (!this.isActive) {
                this.isActive = true;
            } else {
                this.isActive = false;
            }
        }
    }
}

</script>

<style lang="scss" scoped>
    @import "../assets/scss/partials/_variables.scss";

    section {
        .right-side {
            justify-content: flex-end;
            align-items: flex-end;
            .green-button {
                width: 100px;
                margin-bottom: 1em;
                &:hover {
                    cursor: pointer;
                }
            }
        }
        .box {
            position: relative;
            margin-top: 2em;
            .opacity-box {
                border-radius: 20px;
                overflow: hidden;
                background-color: #121117;
                img {
                    width: 100%;
                    opacity: 0.5;
                }
                h4 {
                    position: absolute;
                    bottom: 10%;
                    padding: 0 1.5em;
                    color: $whiteFontColor;
                    font-size: 1.7em;
                }
            }
        }
    }
</style>