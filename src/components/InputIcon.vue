<template>
    <div class="row mb-5">
        <form class="col-md-5">
            <small v-text="labelTitle1"></small>
            <div class="d-flex flex-column">
                <label for="iDefault11">Label</label>
                <span  :style="iconLeft" v-html="iLeft" @click="changeIconLeft"></span>
                <input type="text" name="iDefault11" id="iDefault11" placeholder="Placeholder">
            </div>
        </form>
        <form class="col-md-5">
            <small v-text="labelTitle2"></small>
            <div class="d-flex flex-column">
                <label for="iDefault12">Label</label>
                <span  :style="iconRight" v-html="iRight" @click="changeIconRight"></span>
                <input type="text" name="iDefault12" id="iDefault12" placeholder="Placeholder">
            </div>
        </form>
    </div>
</template>

<script>
    export default {
        name: 'Input-icon',
        data() {
            const iconsContainer1 = [
                '<i class="fa-solid fa-phone"></i>', 
                '<i class="fa-solid fa-house"></i>', 
                '<i class="fa-solid fa-envelope"></i>', 
                '<i class="fa-solid fa-user"></i>', 
                '<i class="fa-solid fa-location-dot"></i>'
            ]
            const iconsContainer2 = [
                '<i class="fa-solid fa-lock"></i>',
                '<i class="fa-solid fa-magnifying-glass"></i>',
                '<i class="fa-solid fa-check"></i>',
                '<i class="fa-solid fa-arrow-right"></i>',
                '<i class="fa-solid fa-arrow-up"></i>'
            ]
            return {
                labelTitle1: '<Input startIcon />',
                labelTitle2: '<Input endIcon />',
                iconLeft: {
                    color: '#828282', 
                    position: 'absolute', 
                    marginTop: '50px', 
                    marginLeft: '10px'
                },
                iconRight: {
                    color: '#828282', 
                    position: 'absolute', 
                    marginTop: '50px', 
                    marginLeft: '170px'
                },
                iconsContainer1,
                iconsContainer2,
                iLeft: '<i class="fa-solid fa-phone"></i>',
                iRight: '<i class="fa-solid fa-lock"></i>',
                numLeft: 0,
                numRight: 0,
            }
        },
        methods: {
            changeIconLeft() {
                this.numLeft === 4 ? this.numLeft = this.numLeft - 4 : this.numLeft = this.numLeft + 1,
                this.iLeft = this.iconsContainer1[this.numLeft]
            },
            changeIconRight() {
                this.numRight === 4 ? this.numRight = this.numRight - 4 : this.numRight = this.numRight + 1,
                this.iRight = this.iconsContainer2[this.numRight]
            }
        }
    }
</script>

<style scoped>
#iDefault11 {
    padding-left: 40px;
}

@media screen and (max-width: 768px) {
    #iDefault11 {
        margin-bottom: 42px;
    }
}
</style>