<template>
    <div class="row mb-5">
        <div class="col-md-5">
            <small v-text="labelTitle1"></small>
            <form class="d-flex flex-column">
                <label for="iDefault7">Label</label>
                <input type="text" name="iDefault7" id="iDefault7" placeholder="Placeholder">
            </form>
        </div>
        <div class="col-md-5">
            <small v-text="labelTitle2"></small>
            <form class="d-flex flex-column">
                <label for="iDefault8">Label</label>
                <input type="text" name="iDefault8" id="iDefault8" placeholder="Placeholder">
            </form>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Input-size',
        data() {
            return {
                labelTitle1: '<Input size=”sm” />',
                labelTitle2: '<Input size=”md” />'
            }
        }
    }
</script>

<style scoped>
#iDefault7 {
    height: 40px;
}

@media screen and (max-width: 768px) {
    #iDefault7 {
        margin-bottom: 42px;
    }
}
</style>