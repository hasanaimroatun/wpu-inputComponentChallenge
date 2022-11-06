<template>
    <div class="row mb-5">
        <div class="col-md-4">
            <small v-text="labelTitle1"></small>
            <div class="d-flex flex-column">
                <label for="iDefault4">Label</label>
                <input type="text" name="iDefault4" id="iDefault4" placeholder="Placeholder">
                <small class="helper">Some interesting text</small>
            </div>
        </div>
        <div class="col-md-4">
            <small v-text="labelTitle2"></small>
            <div class="d-flex flex-column">
                <label for="iDefault5">Label</label>
                <input type="text" name="iDefault5" id="iDefault5" placeholder="Placeholder">
                <small class="helper">Some interesting text</small>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Input-helperText',
        data() {
            return {
                labelTitle1: '<Input helperText=”Some interesting text” />',
                labelTitle2: '<Input helperText=”Some interesting text” error />'
            }
        }
    }
</script>

<style scoped>

</style>