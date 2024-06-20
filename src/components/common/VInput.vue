<template>
    <input type="text">
</template>
<script>
export default {
    name:'VInput'
}
</script>
<style scoped>
    input{
        border: none;
        background-color:#edede9 ;
        border-radius: 20px;
        height: 35px;
        padding-left: 10px;
    }
    input[type=text]:focus{
        outline: 1px solid #2b2d42
    }
</style>