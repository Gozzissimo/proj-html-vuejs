<template>
    <section>
        <div class="container">
            <div class="row box-container d-flex">
                <div class="col-4 box d-flex">
                    <h3>our business areas</h3>
                    <h2>logistics services</h2>
                    <p>We are leaders in providing logistics services with a set of cutting edge technologies and a team of experienced and renowned professionals</p>
                    <ul class="tags list-inline">
                        <li class="green-tag">tradition</li>
                        <li class="green-tag">quality</li>
                        <li class="green-tag">security</li>
                    </ul>
                    <a href="#"><button class="green-button">read more</button></a>
                </div>
                <div class="col-4 box white-box">
                    <div class="gallery-img">
                        <img src="../assets/img/gallery-3.jpg" alt="graphics on phone">
                    </div>
                    <h4>Technology</h4>
                    <p>Focused on developing technology solutions adapted to our client's needs.</p>
                </div>
                <div class="col-4 box white-box">
                    <div class="gallery-img">
                        <img src="../assets/img/gallery-5.jpg" alt="graphics on phone">
                    </div>
                    <h4>Transport</h4>
                    <p>We develop operational strategies to improve logistical efficiency.</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Services",
}
</script>

<style lang="scss" scoped>
    @import "../assets/scss/partials/_variables.scss";

    section {
        background-color: $lightBgColor;
        .box-container {
            justify-content: space-between;
        }
        .box {
            width: calc((100% / 3) - 30px);
            &:first-child {
                flex-direction: column;
                justify-content: space-between;
            }
            &:nth-child(2) {
                margin: 0 30px;
            }
            &:not(:first-child) {
                background-color: $whiteFontColor;
                border-radius: 10px;
                padding: 3em;
            } 
            .green-tag {
                margin-right: 10px;
            }
            .gallery-img {
                img {
                    width: 100%;
                }
            }
            p {
                margin: 0;
            }
            h4 {
                margin: 1em 0;
            }
        }
    }
</style>
