<template>
    <div class="row mb-5">
        <div class="col-md-5">
            <small v-text="labelTitle1"></small>
            <form class="d-flex flex-column iHelper1">
                <label for="iDefault4">Label</label>
                <input type="text" name="iDefault4" id="iDefault4" placeholder="Placeholder" aria-describedby="helpBlock" v-model="iValue1" @input="changeHelper1">
                <div class="helper1 form-text" id="helpBlock" :style="helperColor1">Some interesting text</div>
            </form>
        </div>
        <div class="col-md-5">
            <small v-text="labelTitle2"></small>
            <form class="d-flex flex-column iHelper2">
                <label for="iDefault5" class="labelError">Label</label>
                <input type="text" name="iDefault5" id="iDefault5" placeholder="Placeholder" aria-describedby="helpBlock2" v-model="iValue2" @input="changeHelper2">
                <div class="helper2 form-text" id="helpBlock2" :style="helperColor2">Some interesting text</div>
            </form>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Input-helperText',
        data() {
            return {
                labelTitle1: '<Input helperText=”Some interesting text” />',
                labelTitle2: '<Input helperText=”Some interesting text” error />',
                helperColor1: {
                    display: 'none'
                },
                helperColor2: {
                    display: 'none'
                },
                iValue1: '',
                iValue2: ''
            }
        },
        methods: {
            changeHelper1() {
                this.iValue1.length === 0 ? this.helperColor1.display = 'none' : this.helperColor1.display = 'block'
            },
            changeHelper2() {
                this.iValue2.length === 0 ? this.helperColor2.display =  'none' : this.helperColor2.display = 'block'
            }

        }
    }
</script>

<style scoped>
#iDefault4 {
    border: 1px solid #828282;
}

#iDefault5 {
    border: 1px solid #D32F2F;
}

.helper1,
.helper2 {
    font-family: 'Noto Sans', sans-serif;
    font-weight: 400;
    font-size: 10px;
    line-height: 14.48px;
}

.helper1 {
    color: #828282;
    margin-top: 4px;
}

.labelError {
    color: #D32F2F;
}

.helper2 {
    color: #D32F2F;
    margin-top: 4px;
}

@media screen and (max-width: 768px) {
    .iHelper1 {
        margin-bottom: 42px;
    }
}
</style>