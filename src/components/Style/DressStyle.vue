<template>
    <div class="style">
        <h3>BROWSE BY DRESS STYLE</h3>
        
            <div class="img-top">
            <div class="img-top-right">
                <div class="title">
                    <p>Casual</p>
                </div>
                <img src="../../assets/s1.png">
            </div>
            
            <div class="img-top-left">
                <div class="title">
                    <p >Formal</p>
                </div>
                <img src="../../assets/s2.png">
            </div>
        </div>
        <div class="img-bottom">
            <div class="img-top-right">
                <div class="title">
                    <p>Party</p>
                </div>
                <img src="../../assets/s3.png">
            </div>
            <div class="img-top-right">
                <div class="title">
                    <p>Gym</p>
                </div>
                <img src="../../assets/s4.png">
            </div>
        
        </div>
        
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.img-top{
    margin-top: 60px;
    padding: 0 50px;
    display: flex;
    justify-content: center;
    gap: 30px
}

.img-bottom{
    margin-top: 30px;
    padding: 0 50px;
    display: flex;
    justify-content: center;
    gap: 30px;
}
img{
    height: 289px;
    border-radius: 15px;
    background-position: 50%;
    cursor: pointer;
    padding-left: 0;
}
h3{
    font-family: Integral CF, sans-serif;
    letter-spacing: -.07em;
    font-size: 48px;
    font-weight: 800;
    line-height: 57.6px;
    text-align: center;
}
.title{
    position: absolute;
    margin-top: 20px;
    margin-left: 30px;
    font-family: Satoshi, sans-serif;
    font-size: 36px;
    font-weight: 700;
    line-height: 48.6px;
    text-align: left;
}

.style{
    height: fit-content;
    background-color: #f0f0f0;
    padding: 80px 0;
    margin: 0 100px;
    border-radius: 30px;
}


</style>