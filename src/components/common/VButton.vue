<template>
    <button :style>
        <slot></slot>
    </button>
</template>
<script setup>
defineOptions({
    name:"VButton"
})

const props = defineProps({
    style:Object
})
</script>
<style scoped>
    button{
        border: none;
        border-radius: 25px;

        padding: 7px 20px;
        
        color: white;

        background-color: white;
        transition: all 0.3s
    }
    button:hover{
        background-color: #c5c5c5;
        transition: all 0.3s
    }
</style> 
