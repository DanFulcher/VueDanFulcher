<template>
    <div class="contact">
        <InnerHero title="Contact Me" subTitle="If you have any questions, or are interested in working with me..." para="Feel free to get in touch!" />
        <ContactForm />
    </div>
</template>

<script>
    import InnerHero from '@/components/InnerHero';
    import ContactForm from '@/components/ContactForm';

    export default {
        name: "contact.vue",
        components: {
            InnerHero,
            ContactForm
        }
    }
</script>

<style scoped>

</style>