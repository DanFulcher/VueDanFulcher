<template>
    <a :href="this.link" class="button">
        {{ this.text }}
    </a>
</template>

<script>
    export default {
        name: "Button",
        props: {
            text: String,
            link: String
        }
    }
</script>

<style scoped lang="scss">
    .button {
        background:linear-gradient(135deg, #498bc9 0%, #3ecbbf 100%);
        width: 25%;
        border-radius: .5rem;
        padding: 1rem 1rem;
        border: 1px solid #fff;
        text-align: left;
        color: #fff;
        font-size: 1rem;
        position: relative;
        z-index: 1;
        text-decoration: none;
        display:block;
        &:hover {
            background:#fff;
            color:#498bc9;
            border:1px solid #498bc9;
        }
    }
</style>