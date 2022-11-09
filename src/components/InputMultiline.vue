<template>
    <div>
        <small v-text="labelTitle"></small>
        <form class="d-flex flex-column mb-4">
            <label for="iDefault10">Label</label>
            <textarea name="iDefault10" id="iDefault10" rows="4" placeholder="Placeholder"></textarea>
        </form>
    </div>
</template>

<script>
    export default {
        name: 'Input-multiline',
        data() {
            return {
                labelTitle: '<Input multiline row=”4” />',
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