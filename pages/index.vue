<template>
    <div class='page'>
        {{host}}
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
    async asyncData ({ req, res }) {
        if (process.server) {
            return { host: "Server:" + req.headers.host }
        } else {
            return { host: "Client:" + window.location.host }
        }
    }
}
</script>

<style>

</style>
