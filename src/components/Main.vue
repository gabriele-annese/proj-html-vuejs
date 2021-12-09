<template>
    <div>
        <Hero />
        <GridMarketing />
        <Analysis />
    </div>
</template>

<script>
import Hero from './Hero.vue'
import GridMarketing from './GridMarketing.vue'
import Analysis from './Analysis.vue'
export default {
name: 'Main',
components: {
    Hero,
    GridMarketing,
    Analysis,
}
}
</script>

<style lang="scss" scoped>

</style>