<template>
    <div>
        <small v-text="labelTitle"></small>
        <div class="d-flex flex-column mb-5">
            <label for="iDefault9">Label</label>
            <input type="text" name="iDefault9" id="iDefault9" placeholder="Text">
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Input-fullWidth',
        data() {
            return {
                labelTitle: '<Input fullWidth />'
            }
        }
    }
</script>

<style scoped>
#iDefault9 {
    width: 98%;
}

input, 
input::placeholder {
    color: #333333;
}
</style>