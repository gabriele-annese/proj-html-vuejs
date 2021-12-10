<template>
    <div>
        <Hero />
        <GridMarketing />
        <Analysis />
        <GridBusiness />
        <Testimonials />
        <GrdiPost />
    </div>
</template>

<script>
import Hero from './Hero.vue'
import GridMarketing from './GridMarketing.vue'
import Analysis from './Analysis.vue'
import GridBusiness from './GridBusiness.vue'
import Testimonials from './Testimonials.vue'
import GrdiPost from './GrdiPost.vue'
export default {
name: 'Main',
components: {
    Hero,
    GridMarketing,
    Analysis,
    GridBusiness,
    Testimonials,
    GrdiPost,
}
}
</script>

<style lang="scss" scoped>

</style>