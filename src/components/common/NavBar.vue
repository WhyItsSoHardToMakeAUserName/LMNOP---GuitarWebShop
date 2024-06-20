<template lang="">
    <div class="container">

        <div class="block">

            <img class="menu-icon" src="@/images/menu-2-outline.svg">

        </div>
        
        <div class="block search">

            <VInput style="width:100%"></VInput>
            <VButton class="filter-dropdown"><img  class="filter-dropdown-img"src="@/images/arrow-upward-outline.svg"></VButton>

        </div>

        <div class="block">
            <VButton><img  class="filter-dropdown-img"src="@/images/person-outline.svg"></VButton>
        </div>
    </div>
</template>
<script setup>
defineOptions({
    name:"NavBar"
})

import { ref } from 'vue'

const input = ref()

</script>
<style scoped>
    .container{
        width:100%;
        display: flex;
        align-items: center;
        justify-content: space-between;
        margin: 10px
    }
    .block{
        display: flex;
        align-items: center
    }
    .search{
        width: 50%;
    }
    .menu-icon{
        width: 40px;
        filter: invert(25%) sepia(30%) saturate(433%) hue-rotate(97deg) brightness(92%) contrast(87%);
    }


    .filter-dropdown-img{
        width: 30px;
    }
    .filter-dropdown{
        padding: 5px;
        margin: 0px 5px;
        height: 40px;
    }
</style>