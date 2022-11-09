<template>
    <div>
        <small v-text="labelTitle"></small>
        <form class="d-flex flex-column mb-5">
            <label for="iDefault3">Label</label>
            <input type="text" name="iDefault3" id="iDefault3" placeholder="Placeholder" disabled>
        </form>
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
input {
    border: 1px solid #E0E0E0;
    background-color: #F2F2F2;
}
</style>