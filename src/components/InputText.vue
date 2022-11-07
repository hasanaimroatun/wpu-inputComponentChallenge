<template>
    <div>
        <small v-text="labelTitle"></small>
        <div class="d-flex flex-column mb-5">
            <label for="iDefault6">Label</label>
            <input type="text" name="iDefault6" id="iDefault6" placeholder="Text">
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Input-text',
        data() {
            return {
                labelTitle: '<Input value=”text” />'
            }
        }
    }
</script>

<style scoped>
input::placeholder {
    color: #333;
}
</style>