<template>
    <div>
        <small v-text="labelTitle"></small>
        <form class="d-flex flex-column mb-5">
            <label for="iDefault1" :style="{color: colorText}">Label</label>
            <input 
                type="text" 
                name="iDefault1" 
                id="iDefault1" 
                placeholder="Placeholder"
                @mouseenter="changeColorGrey"
                @mouseleave="changeColorDefault"
                @focus="changeColorBlue"
                @input="changeColorBlue">
        </form>
    </div>
</template>

<script>
    export default {
        name: 'Input-default',
        data() {
            return {
                labelTitle: '<Input />',
                colorText: '#828282'
            }
        },
        methods: {
            changeColorBlue() {
                this.colorText = '#2962FF'
            },
            changeColorGrey() {
                this.colorText = '#333333'
            },
            changeColorDefault() {
                this.colorText = '#828282'
            }
        }
    }
</script>

<style scoped>
input:hover {
    border: 1px solid #333333;
}

input:focus {
    border: 1px solid #2962FF;
}
</style>