<template>
<div id="app" class="layout-row">
    <NavMenu />
    <div id="main" class="layout-column flex">
        <Header />
        <div class="content">
            <div>
                <div class="page-hero page-container " id="page-hero">
                    <div class="padding d-flex">
                        <router-view />
                    </div>
                </div>
            </div>
        </div>
        <div id="footer" class="page-footer hide">
            <div class="d-flex p-3">
                <span class="text-sm text-muted flex">&copy; Copyright. flatfull.com</span>
                <div class="text-sm text-muted">Version 1.1.2</div>
            </div>
        </div>
    </div>

</div>
</template>

<script>
import NavMenu from '@/components/NavMenu.vue'
import Header from '@/components/Header.vue'

export default {
  name: 'App',
  components: {
    NavMenu,
    Header
    },
mounted() {
    init_basik()
}
}
</script>

<style lang="scss">
#app {
    width: 100%;
    height: 100vh
}
</style>
