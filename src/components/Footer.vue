<template>
    <section class="footer">
        <div class="container">
            <p>&copy; Copyright Dan Fulcher {{ this.date }}</p>
        </div>
    </section>
</template>

<script>
    export default {
        name: "footer.vue",
        data: function () {
            return {
                date: ''
            }
        },
        methods: {
            getDate() {
                this.date = new Date().getFullYear()
            }
        },
        beforeMount() {
            this.getDate()
        }
    }
</script>

<style scoped>

</style>