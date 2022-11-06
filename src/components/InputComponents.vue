<template>
    <div class="row">
        <div class="col-2 offset-1 text-start">
            <Navigation />
        </div>
        <div class="col-9 text-start">
            <Inputs />
        </div>
    </div>
</template>

<script>
import Navigation from './Navigation.vue'
import Inputs from './Inputs.vue'

    export default {
        name: "input-components",
        components: {
            Navigation,
            Inputs
        }
    }
</script>

<style>

</style>