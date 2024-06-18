<template>
    <div class="product-infor">
        <img :src="data.img">
        <div class="product">
            <p class="product-name">{{ data.productName }}</p>
            <div class="product-rate">
                <v-rating
                    v-model="data.rating"
                    active-color="yellow-darken-2"
                    :half-increments="true"
                    color="white"
                    :length="5"
                    density="compact"
                    readonly
            ></v-rating>
                <p>{{ data.rating }}/5</p>
            </div>
            <div class="product-price">
                <p>${{ data.price }}</p>
                <p v-if="data.oldPrice" class="old-price">${{ data.oldPrice }}</p>
                <div v-if="data.promo" class="promo">{{ data.promo }}%</div>
            </div>
        </div>
    </div>
</template>

<script>
import CustomRate from '../item/CustomRate.vue'
import CustomRateVue from '../item/CustomRate.vue'
export default {
  components: { CustomRate },
    component:{
        CustomRateVue
    },
    props: {
        data: {
            type: Object,
            required: true
        }
    }
}
</script>

<style scoped>
img{
    border-radius: 20px;
    width: 295px;
    height: 298px;
    object-fit: cover;
}
.product-infor{
    margin-top:10px ;
}

.product{
    display: flex;
    flex-direction: column;
    text-align: left;
}
.product-name{
    margin-top: 10px;
    font-family: Satoshi, sans-serif;
    font-size: 15px;
    font-weight: 700;
    line-height: 27px;
    text-align: left;
}

.product-rate{
    display: flex;
    font-family: "Satoshi";
    font-size: 18px;
    font-weight: 400;
    align-items: center;
}
.product-price{
    font-family: "Satoshi";
    font-size: 24px;
    font-weight: 800;
    display: flex;
    align-items: center;
}
.product-price p{
    margin: 30px;
    margin-left: 0px;
}
.promo{
    width: 58px;
    height: 28px;
    padding: 6px 14px 6px 14px;
    gap: 12px;
    border-radius: 62px;
    background: #FF33331A;
    color: #FF3333;
    font-size: 12px;
    font-weight: 500;
    line-height: 16.2px;
    text-align: center;
}
.old-price{
    text-decoration-line:line-through
}
</style>