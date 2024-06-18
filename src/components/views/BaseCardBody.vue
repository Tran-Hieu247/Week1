<template>
    <div>
        <poster-component></poster-component>
        <brand-item></brand-item>
        <product-view name="NEW ARRIVALS" :data="data1"></product-view>
        <v-divider></v-divider>
        <product-view name="TOP SELLING" :data="data2"></product-view>
        <dress-style></dress-style>
        <view-custom></view-custom>
        <infor-customer></infor-customer>
    </div>
</template>
<script>
import BrandItem from '../Brand/BrandItem.vue'
import PosterComponent from '../Poster/PosterComponent.vue'
import ProductView from '../Product/ProductView.vue'
import data1 from '../../assets/data1.json'
import data2 from '../../assets/data2.json'
import DressStyle from '../Style/DressStyle.vue'
import ViewCustom from '../Customer/ViewCustom.vue'
import InforCustomer from '../Customer/InforCustomer.vue'
export default {
    components:{
        PosterComponent,
        BrandItem,
        ProductView,
        DressStyle,
        ViewCustom,
        InforCustomer
    }
    ,
    data(){
        return{
            data1: data1,
            data2: data2
        }
    }
}
</script>
