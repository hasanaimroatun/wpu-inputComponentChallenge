<template>
    <div>
        <small v-text="labelTitle"></small>
        <div class="d-flex flex-column mb-5">
            <label for="iDefault3">Label</label>
            <input type="text" name="iDefault3" id="iDefault3" placeholder="Placeholder">
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Input-disabled',
        data() {
            return {
                labelTitle: '<Input disabled/>'
            }
        }
    }
</script>

<style scoped>

</style>