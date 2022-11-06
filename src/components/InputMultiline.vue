<template>
    <div>
        <small v-text="labelTitle"></small>
        <div class="d-flex flex-column mb-4">
            <label for="iDefault10">Label</label>
            <textarea name="iDefault10" id="iDefault10" rows="10" placeholder="Placeholder"></textarea>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Input-multiline',
        data() {
            return {
                labelTitle: '<Input multiline row=”4” />'
            }
        }
    }
</script>

<style scoped>
#iDefault10 {
    width: 200px;
    border-radius: 8px;
}
</style>