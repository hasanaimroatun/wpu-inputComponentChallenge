<template>
    <div class="row">
        <div class="col-3 offset-1 text-start">
            <Navigation />
        </div>
        <div class="col-8 text-start">
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
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@500;700&family=Noto+Sans:wght@400;500;700&family=Poppins:wght@500;600&family=Ubuntu+Mono&display=swap');

</style>