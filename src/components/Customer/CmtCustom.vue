<template>
    <div class="customer-item">
        <div class="rating">
            <v-rating
            v-model="data.rating"
            active-color="yellow-darken-2"
            :half-increments="true"
            color="white"
            :length="5"
            density="compact"
            readonly
        ></v-rating>
        </div>
    
        <div class="name">
            <p class="name-text">{{data.name}}</p>
            <img src="../../assets/greenTick.png">
        </div>
        
        <p class="comment">{{data.comment}}</p>
    </div>
</template>
<script>
export default {
    props: {
        data: {
            type: Object,
            required: true
        }
    }
}
</script>
<style scoped>
.customer-item{
    border: 1px solid #c7c8cc;
    min-width: 297px;
    padding: 20px;
    border-radius: 20px;
}
v-rating{
    width: 139;
    height: 23;
    fill: none;
}
.name-text{
    font-family: Satoshi, sans-serif;
    font-size: 20px;
    font-weight: 700;
    line-height: 22px;
    text-align: left;
}

.comment{
    font-family: Satoshi, sans-serif;
    font-size: 16px;
    font-weight: 400;
    line-height: 22px;
    text-align: left;
    color: #000;
    opacity: 60%;
    padding-top: 15px;
}
.rating{
    display: flex;
    justify-content: left;
}
img{
    display: flex;
    padding-top:0 ;
}

.name{
    display: flex;
    padding-top: 15px;
}
</style>