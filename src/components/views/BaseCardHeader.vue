<template>
    <div class="header">
        <notify-header></notify-header>
        <div class="headerBar">
            <logo-header logoName="SHOP.CO"></logo-header>
            <header-navbar></header-navbar>
            <search-navbar></search-navbar>
            <div class="btnGroup">
                <v-icon icon="mdi mdi-cart"></v-icon>
                <v-icon icon="mdi mdi-account-circle-outline"></v-icon>
                
            </div>
        </div>
    </div>
        
        
</template>
<script>
import HeaderNavbar from '../navbar/HeaderNavbar.vue';
import LogoHeader from '../Logo/LogoHeader.vue';
import NotifyHeader from '../Notify/NotifyHeader.vue';
import SearchNavbar from '../navbar/SearchNavbar.vue';
export default {
    components:{
        NotifyHeader,
        LogoHeader,
        HeaderNavbar,
        SearchNavbar
    }
}
</script>
<style scoped>
    .headerBar{
        display: flex;
        padding: 20px 50px;
        align-items: center;
        justify-content: space-between;
    }
.headerBar{
    display: flex;
    text-align: center;
}
</style>