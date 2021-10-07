<template>
    <div id='header'>
        <div class='container'>
            <Topbar @sidenavtoggle="displaySidebar = !displaySidebar"/>
        </div>
    </div>
</template>

<script>
import Topbar from '@/components/page/_common/Topbar.vue'

export default {
  components: {
    Topbar
  },
}
</script>

<style scoped>
    .container {
        padding-bottom: 0px;
    }
</style>
