<template>
    <div class="product-view">
        <h3> {{name}}</h3>
        <section>
            <product-infor v-for="item in data" :key="item" :data="item" ></product-infor>
        </section>
        <button>View All</button>
    </div>
</template>

<script>
import ProductInfor from './ProductInfor.vue'
export default {
    components:{
        ProductInfor
    },
    props:{
        name: {
            type: String,
            required: true
        },
        data: {
            type: Array,
            required: true
        }
    }
}
</script>

<style scoped>
section{
    display: flex;
    height: 30%;
    justify-content: space-around;
    padding: 1rem 0;
    width: 100%;
    z-index: 0;
}

product-infor{
    display: block;
    margin: 20px;
}
button{
    margin-top: 30px;
    margin-bottom: 20px;
    width: 218px;
    height: 52px;
    border-radius: 62px;
    border: 1px solid #0000001A
}
h3{
    margin-top: 72px;
    font-family: Integral CF, sans-serif;
    letter-spacing: -.07em;
    font-size: 48px;
    font-weight: 800;
    line-height: 57.6px;
    text-align: center;
    color: black;
}

</style>