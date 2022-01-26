<template>
    <main>
        <Services />
        <Company />
        <Customers />
        <News />
        <Newsletter />
        <ContactForm />
    </main>
</template>

<script>
import Services from './Services.vue'
import Company from './Company.vue'
import Customers from './Customers.vue'
import News from './News.vue'
import Newsletter from './Newsletter.vue'
import ContactForm from './ContactForm.vue'

export default {
    name: "Main",
    components: {
        Services,
        Company,
        Customers,
        News,
        Newsletter,
        ContactForm,
    },
}
</script>

<style lang="scss">
    @import "../assets/scss/partials/_variables.scss";

    section {
        padding: 8em;
        h2 {
            text-transform: capitalize;
            font-weight: 800;
            font-size: 3em;
        }
        h3 {
            text-transform: uppercase;
            color: $greenFontColor;
            font-size: 0.8em;
            font-weight: bold;
        }
        h4 {
            font-size: 1.3em;
            font-weight: bold;
        }
        p {
            color: $greyFontColor;
        }
    }
</style>