<template>
    <div>
        <small v-text="labelTitle"></small>
        <div class="d-flex flex-column mb-5">
            <label for="iDefault2">Label</label>
            <input type="text" name="iDefault2" id="iDefault2" placeholder="Placeholder">
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Input-error',
        data() {
            return {
                labelTitle: '<Input error/>'
            }
        }
    }
</script>

<style scoped>

</style>