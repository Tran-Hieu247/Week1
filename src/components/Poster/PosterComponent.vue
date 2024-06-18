<template>
    <div class="poster">
        <div class="msg-poster">
            <p class="text1">FIND CLOTHES THAT MATCHES YOUR STYLE</p>
            <p class="text2">Browse through our diverse range of meticulously crafted garments, designed to bring out your individuality and cater to your sense of style.</p>
            <button>Shop Now</button>
            <div class="posterInfor">
                <poster-infor val="200" msg="International Brands"></poster-infor>
                <poster-infor val="2,000" msg="High-Quality Products"></poster-infor>
                <poster-infor val="30,000" msg="Happy Customers"></poster-infor>
            </div>
        </div>

        <div class="img-poster">
            <img src="../../assets/Poster.png" class="img">
        </div>
    </div>
</template>

<script>
import PosterInfor from './PosterInfor.vue'
export default {
    components:{
        PosterInfor
    }
}
</script>

<style scoped>
.poster {
    display: flex;
    width: 100%;
}
.msg-poster {
    width: 50%;
    background: #F2F0F1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;   
    text-align: left; 
    padding: 0px 0px 0px 60px;
}
.img-poster {
    width: 50%;
    height: 663px;
    position: relative;
}
.posterInfor{
    width: 100%;
    height: 74px;
    display: flex;
    flex-wrap: wrap;
    justify-content: left;
    margin: 30px 0;
    margin-top: 0;
    
}


.img{
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: 50% 0%;
}
button{
    padding: 16px 54px 16px 54px;
    border-radius: 30px;
    background: #000;
    color: #fff;
    margin-bottom: 40px;
}
.text1{
    max-width: 577px;
    font-family: Integral CF, sans-serif;
    letter-spacing: -.09em;
    font-size: 64px;
    font-weight: 800;
    line-height: 64px;
    text-align: left;
    margin: 100px 0 40px 0;
    padding-top: 0px;
    color: #000000;
}

.text2{
    max-width: 545px;
    height: 33px;
    font-family: Satoshi, sans-serif;
    font-size: 16px;
    font-weight: 400;
    line-height: 22px;
    text-align: left;
    opacity: 60%;
    margin:30px 0;
    margin-top:0;
    color: #00000099;



}
</style>