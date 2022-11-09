<template>
    <div>
        <small v-text="labelTitle"></small>
        <form class="d-flex flex-column mb-5">
            <label for="iDefault2" :style="{color: colorText}">Label</label>
            <input 
                type="text" 
                name="iDefault2" 
                id="iDefault2" 
                placeholder="Placeholder"
                @mouseenter="changeColorGrey"
                @mouseleave="changeColorRed"
                @focus="changeColorRed"
                @input="changeColorRed">
        </form>
    </div>
</template>

<script>
    export default {
        name: 'Input-error',
        data() {
            return {
                labelTitle: '<Input error/>',
                colorText: '#D32F2F'
            }
        },
        methods: {
            changeColorGrey() {
                this.colorText = '#333333'
            },
            changeColorRed() {
                this.colorText = '#D32F2F'
            }
        }
    }
</script>

<style scoped>
input {
    border: 1px solid #D32F2F;
}

input:hover {
    border: 1px solid #333333;
}

input:focus {
    border: 1px solid #D32F2F;
}
</style>