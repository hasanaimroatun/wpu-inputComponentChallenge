<template>
    <div class="row mb-5">
        <div class="col-md-5">
            <small v-text="labelTitle1"></small>
            <div class="d-flex flex-column">
                <label for="iDefault4">Label</label>
                <input type="text" name="iDefault4" id="iDefault4" placeholder="Placeholder">
                <div class="helper1">Some interesting text</div>
            </div>
        </div>
        <div class="col-md-5">
            <small v-text="labelTitle2"></small>
            <div class="d-flex flex-column">
                <label for="iDefault5">Label</label>
                <input type="text" name="iDefault5" id="iDefault5" placeholder="Placeholder">
                <div class="helper2">Some interesting text</div>
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
.helper1,
.helper2 {
    font-family: 'Noto Sans', sans-serif;
    font-weight: 400;
    font-size: 10px;
    line-height: 14.48px;
}

.helper1 {
    color: #828282;
}

.helper2 {
    color: #D32F2F;
}
</style>