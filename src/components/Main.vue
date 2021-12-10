<template>
    <div>
        <Hero />
        <GridMarketing />
        <Analysis />
        <GridBusiness />
    </div>
</template>

<script>
import Hero from './Hero.vue'
import GridMarketing from './GridMarketing.vue'
import Analysis from './Analysis.vue'
import GridBusiness from './GridBusiness.vue'
export default {
name: 'Main',
components: {
    Hero,
    GridMarketing,
    Analysis,
    GridBusiness
}
}
</script>

<style lang="scss" scoped>

</style>