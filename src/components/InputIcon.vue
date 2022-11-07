<template>
    <div class="row mb-5">
        <div class="col-md-5">
            <small v-text="labelTitle1"></small>
            <div class="d-flex flex-column">
                <label for="iDefault11">Label</label>
                <font-awesome-icon icon="fa-solid fa-phone" class="fa-lg" :style="iconLeft"/>
                <input type="text" name="iDefault11" id="iDefault11" placeholder="Placeholder">
            </div>
        </div>
        <div class="col-md-5">
            <small v-text="labelTitle2"></small>
            <div class="d-flex flex-column">
                <label for="iDefault12">Label</label>
                <font-awesome-icon icon="fa-solid fa-lock" class="fa-lg" :style="iconRight" />
                <input type="text" name="iDefault12" id="iDefault12" placeholder="Placeholder">
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Input-icon',
        data() {
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
                }
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