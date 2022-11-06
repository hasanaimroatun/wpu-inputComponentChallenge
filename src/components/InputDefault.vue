<template>
    <div>
        <small v-text="labelTitle"></small>
        <div class="d-flex flex-column mb-5">
            <label for="iDefault1">Label</label>
            <input type="text" name="iDefault1" id="iDefault1" placeholder="Placeholder">
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Input-default',
        data() {
            return {
                labelTitle: '<Input />'
            }
        }
    }
</script>

<style scoped>

</style>