<template>
    <div class='page'>
        <Header />
        <Hero />
    </div>
</template>

<script>
import Header from '@/components/page/_common/Header.vue'
import Hero from '@/components/page/home/SKHero.vue'

export default {
    layout: 'defaultPage',
        components: {
            Header, Hero,
    },
}
</script>

<style>

</style>
