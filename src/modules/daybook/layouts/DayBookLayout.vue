<template>
    <Navbar />
    <div class="d-flex">
        <div class="col-4">
            <EntityList />
        </div>
        <div class="col">
            <router-view></router-view>
        </div>
    </div>

</template>

<script>
import { defineAsyncComponent } from '@vue/runtime-core'



export default {
    components: {
        Navbar: defineAsyncComponent(() => import("../components/Navbar.vue")),
        EntityList: defineAsyncComponent(() => import("../components/EntityList.vue"))
    }
}
</script>

<style>

</style>