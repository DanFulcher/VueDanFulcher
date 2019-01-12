<template>
    <div class="work">

        <InnerHero title="My Work" subTitle="Aside from the beauty of a site you're currently viewing." para="Here’s some examples of other work that I’ve designed and built." />

        <WorkRepeater />

        <CallToAction />

    </div>
</template>

<script>
    import InnerHero from '@/components/InnerHero.vue'
    import WorkRepeater from '@/components/WorkRepeater.vue'
    import CallToAction from '@/components/CallToAction.vue'

    export default {
        name: "work.vue",
        components: {
            InnerHero,
            WorkRepeater,
            CallToAction
        }
    }
</script>

<style scoped>

</style>