<template>
    <div class="infoPost">
        <p class="val">{{val}}+</p>
        <p class="msg">{{msg}}</p>
    </div>
</template>

<script>
export default {
    props:['val', 'msg']
}
</script>

<style>
.infoPost {
        height: 74px;
}

.val {
        font-family: Satoshi, sans-serif;
        font-size: 40px;
        font-weight: 700;
        line-height: 54px;
        text-align: left;
}

.msg {
        font-family: Satoshi, sans-serif;
        font-size: 16px;
        font-weight: 400;
        line-height: 22px;
        text-align: left;
        opacity: 60%;
        color: #00000099;
}
@media (max-width: 1024px) {
    .infoPost {
        height: 52px;
    }

    .val {
        font-size: 24px;
        line-height: 32px;
    } 

    .msg {
        font-size: 12px;
    
    }
}
</style>