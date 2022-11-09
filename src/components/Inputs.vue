<template>
    <div>
        <div class="mainTitle">Inputs</div>
        <Input />
        <InputError />
        <InputDisabled />
        <InputHelperText />
        <InputIcon />
        <InputText />
        <InputSize />
        <InputFullWidth />
        <InputMultiline />
        <div class="createdBy mb-5">created by <a href="https://github.com/hasanaimroatun/wpu-inputComponentChallenge.git">hasanaimroatun</a> - devChallenges.io</div>
    </div>
</template>

<script>
import Input from './InputDefault.vue'
import InputError from './InputError.vue'
import InputDisabled from './InputDisabled.vue'
import InputHelperText from './InputHelperText.vue'
import InputIcon from './InputIcon.vue'
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
            InputIcon,
            InputText,
            InputSize,
            InputFullWidth,
            InputMultiline,
        }
    }
</script>

<style>
.mainTitle {
    font-family: 'Poppins', sans-serif;
    font-weight: 500;
    font-size: 24px;
    line-height: 36px;
    color: #4F4F4F;
    margin-bottom: 65px;
}

small {
    font-family: 'Ubuntu Mono', monospace;
    font-weight: 400;
    font-size: 12px;
    line-height: 12px;
    color: #333333;
}

input {
    width: 200px;
    height: 56px;
    border-radius: 8px;
    border: 1px solid #828282;
    padding-left: 12px;
    outline: none;
    margin-top: 4px;
}

input,
input::placeholder,
textarea,
textarea::placeholder {
    font-family: 'Noto Sans', sans-serif;
    font-weight: 500;
    font-size: 14px;
    line-height: 20.27px;
    color: #333;
}

input::placeholder,
textarea::placeholder {
    color: #828282;
}

textarea {
    padding-left: 12px;
    padding-top: 18px;
    margin-top: 4px;
    outline: none;
}

label {
    margin-top: 16px;
    font-family: 'Noto Sans', sans-serif;
    font-weight: 400;
    font-size: 12px;
    line-height: 17.38px;
}

.createdBy {
    font-family: 'Montserrat', sans-serif;
    font-weight: 500;
    font-size: 14px;
    line-height: 17.07px;
    color: #9E9E9E;
}

.createdBy a {
    font-weight: 700;
    color: inherit;
    text-decoration: none;
}

.createdBy a:hover {
    color: #333;
}
</style>