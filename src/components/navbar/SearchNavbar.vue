
<template>
    <div class="searchBox">
        <v-icon icon="mdi mdi-magnify"></v-icon>
        <input class="searchInput" placeholder="Search for products..."/>
    </div>
</template>
<script>
    export default {
        
    }
</script>

<style scoped>

    .searchBox {
        width: 577px;
        height: 48px;
        border-radius: 25px;
        display: flex;
        justify-items: center;
        align-items: center;
        background-color: #f0f0f0;
        padding-left: 20px;
        padding-right: 30px;
        margin-left: auto;
        margin-right: 20px;
    }

    .searchInput {
        border: 1px solid transparent;
        width: 90%;
        padding: 5px 0;
        outline: none;
        background-color: #f0f0f0;
        margin-left: 12px;
        opacity: 60%;
        font-family: Satoshi, sans-serif;
        font-size: 16px;
        font-weight: 400;
        line-height: 21.6px;
        text-align: left;
    }

    .searchInput :focus :active{
        border: none;
    }

    @media (max-width: 748px) {

    }
</style>