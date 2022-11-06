<template>
    <div>
        <div class="mainTitle">Inputs</div>
        <Input />
        <InputError />
        <InputDisabled />
        <InputHelperText />
        <InputText />
        <InputSize />
        <InputFullWidth />
        <InputMultiline />
        <div class="createdBy mb-5">created by <a href="#">hasanaimroatun</a> - devChallenges.io</div>
    </div>
</template>

<script>
import Input from './InputDefault.vue'
import InputError from './InputError.vue'
import InputDisabled from './InputDisabled.vue'
import InputHelperText from './InputHelperText.vue'
import InputText from './InputText.vue'
import InputSize from './InputSize.vue'
import InputFullWidth from './InputFullWidth.vue'
import InputMultiline from './InputMultiline.vue'
    export default {
        name: 'Inputs-container',
        components: {
            Input,
            InputError,
            InputDisabled,
            InputHelperText,
            InputText,
            InputSize,
            InputFullWidth,
            InputMultiline,
        }
    }
</script>

<style>
input {
    width: 200px;
    height: 56px;
    border-radius: 8px;
}

label {
    margin-top: 16px;
}
</style>