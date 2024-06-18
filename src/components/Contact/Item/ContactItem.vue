<template>
    <div>
        <div class="title">{{title}}</div>
        <div class="detail">{{detail1}}</div>
        <div class="detail">{{detail2}}</div>
        <div class="detail">{{detail3}}</div>
        <div class="detail">{{detail4}}</div>
        
    </div>
</template>

<script>
export default {
    props:['title', 'detail1','detail2','detail3','detail4']
}
</script>

<style scoped>
.title{
    font-weight: 600;
    line-height: 18px;
    letter-spacing: 3px;
    margin-bottom: 15px;
}
.detail{
    font-family: Satoshi, sans-serif;
    font-size: 16px;
    text-align: left;
    width: 100%;
    height: 80%;
    font-weight: 400;
    line-height: 27px;
    opacity: 60%;
}
</style>