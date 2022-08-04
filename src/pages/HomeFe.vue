<template>
    <div class="home">
        <div class="wrapper">

            <!-- Preloader -->
            <div class="preloader flex-column justify-content-center align-items-center">
                <img class="animation__shake" src="dist/img/AdminLTELogo.png" alt="AdminLTELogo" height="60" width="60">
            </div>
            <NavbarFe/>
            <SidebarFe/>
            <FooterFe/>
        </div>
    </div>

</template>

<script>

import NavbarFe from '@/components/NavbarFe.vue'
import SidebarFe from '@/components/SidebarFe.vue'
import FooterFe from '@/components/FooterFe.vue'

import Vue from 'vue'
import { BootstrapVue, IconsPlugin } from 'bootstrap-vue'

// Import Bootstrap and BootstrapVue CSS files (order is important)
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

// Make BootstrapVue available throughout your project
Vue.use(BootstrapVue)
// Optionally install the BootstrapVue icon components plugin
Vue.use(IconsPlugin)
export default {
    name : 'HomeFe',

    components: {
        NavbarFe,
        SidebarFe,
        FooterFe
    }
}
</script>

<style>


</style>