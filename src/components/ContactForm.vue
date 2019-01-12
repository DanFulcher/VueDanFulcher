<template>
    <section class="contact-form">
        <div class="container">
            <div class="contact-form__content">
                <h1>Please fill out the simple form below...</h1>
                <p>Or email me direct at me@danfulcher.co.uk<br/>
                I am usually quick to respond, so you won’t be left hanging for long!</p>
                <form id="form" @submit.prevent="submit">
                    <input placeholder="Name" v-model="name" />
                    <input placeholder="Email" v-model="email" />
                    <textarea placeholder="Message" v-model="message"></textarea>
                </form>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "contact-form.vue",
        data: function() {
            return {
                name: '',
                email:'',
                message: '',
                submitted: false
            }
        },
        methods: {
            submit: function() {
                this.submitted = true
            }
        }
    }
</script>

<style scoped lang="scss">
    .contact-form {
        padding:6.25rem 0;
    }
</style>