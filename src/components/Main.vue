<template>
    <div>
        <Hero />
        <GridMarketing />
    </div>
</template>

<script>
import Hero from './Hero.vue'
import GridMarketing from './GridMarketing.vue'
export default {
name: 'Main',
components: {
    Hero,
    GridMarketing,
}
}
</script>

<style lang="scss" scoped>

</style>