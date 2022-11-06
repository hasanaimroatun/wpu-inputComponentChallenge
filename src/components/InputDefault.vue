<template>
    <div>
        <small v-text="labelTitle"></small>
        <div class="d-flex flex-column">
            <label for="iDefault">Label</label>
            <input type="text" name="iDefault" id="iDefault" placeholder="Placeholder">
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