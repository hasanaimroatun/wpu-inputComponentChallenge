<template>
    <div>
        <div class="mainTitle">Inputs</div>
        <Input />
        <InputError />
    </div>
</template>

<script>
import Input from './InputDefault.vue'
import InputError from './InputError.vue'
    export default {
        name: 'Inputs-container',
        components: {
            Input,
            InputError,
        }
    }
</script>

<style scoped>

</style>