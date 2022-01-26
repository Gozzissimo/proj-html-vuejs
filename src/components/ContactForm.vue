<template>
    <section id="contact">
        <div class="container">
            <div class="row">
                <div class="col-8 left-side">
                    <h3>send a message</h3>
                    <h2 class="my-3">get in <span class="green-bg green">touch</span></h2>
                    <p>We will respond to your message as soon as possible.</p>
                    <form class="row g-3 mt-5 needs-validation" action="#">
                        <input class="col-6 grey" placeholder="Name" type="text" name="contact-name" id="contact-name">
                        <input class="col-6 grey" placeholder="Email" type="email" name="contact-name" id="contact-email">
                        <input class="col-6 grey" placeholder="Phone" type="tel" name="contact-name" id="contact-phone">
                        <select class="col-6 grey" name="More Info" id="contact-info">
                            <option >More Info</option>
                            <option value="1">Private</option>
                            <option value="2">Society</option>
                            <option value="3">Corporation</option>
                        </select>
                        <textarea class="col-12 text-box grey" placeholder="Message" name="contact-message" rows="6"></textarea>
                        <input class="green-button col-2" type="submit" value="send">
                    </form>
                </div>
                <div class="col-4 right-side">
                    <h4>Example Inc.</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga molestias atque </p>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga molestias atque </p>
                    <ul>
                        <li>
                            <i class="fas fa-phone-alt"></i>+1 (305) 1234-5678
                        </li>
                        <li>
                            <i class="fas fa-envelope"></i>hello@example.com
                        </li>
                        <li>
                            <i class="fas fa-map-marker-alt"></i>Main Avenue, 987
                        </li>
                    </ul>
                        <a href="#">
                            <button class="borderless-button">view map</button>
                        </a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "ContactForm",
}
</script>

<style lang="scss" scoped>
    @import "../assets/scss/partials/_variables.scss";
    
    section {
        background-color: $lightBgColor;
        .left-side {
            input.grey, select, textarea, option {
            background-color: rgba($greyFontColor, 0.3);
            }
            .text-box {
                height: 120px;
            }
        }
        .right-side {
            padding-left: 3em;
            h4 {
                margin-bottom: 1em;
            }
            ul {
                padding: 0;
                li {
                    color: $greenFontColor;
                    margin-bottom: 1em;
                    font-size: 1.2em;
                    i {
                        padding: 0.6em;
                        background-color: rgba($color: $greenBgColor, $alpha: 0.3);
                        border-radius: 50%;
                        margin-right: 10px;
                    }
                }
            }
            button {
                color: $greenFontColor;
            }
        }
    }
</style>