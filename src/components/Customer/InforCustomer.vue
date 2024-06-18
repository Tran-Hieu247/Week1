<template>
    <div class="upto">
        <div class="title">
            STAY UPTO DATE ABOUT OUR LATEST OFFERS
        </div>
        <div class="infor">
            <div class="email">
                <v-icon icon="mdi mdi-email" color="black"></v-icon>
                <input placeholder="Enter your email address">
                
            </div>
            <div class="subscribe">
                <button>Subscribe to Newsletter</button>
            </div>
            
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.infor{
    width: 50%;
    display: flex;
    flex-direction: column;
    margin: 35px 50px;
    gap: 10px;
}
.title{
    width: 50%;
    font-size: 40px;
    font-family: Integral CF, sans-serif;
    letter-spacing: -.07em;
    font-weight: 800;
    line-height: 40px;
    text-align: left;
    align-content: center;
    padding: 0 50px;
}
.upto{
    margin: 0 100px;
    height: -moz-fit-content;
    height: fit-content;
    border-radius: 20px;
    color: #fff;
    background-color: #000;
    z-index: 2;
    position: relative;
    display: flex;
}

.email{
    width: 100%;
    height: 48px;
    border-radius: 25px;
    display: flex;
    justify-items: center;
    align-items: center;    
    text-align: center;
    background-color: #f0f0f0;
    padding-left: 20px;
    padding-right: 30px;
    margin-left: auto;
    margin-right: 20px;
   
}

input{
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

button{
    height: 48px;
    border-radius: 30px;
    outline: none;
    font-family: Satoshi, sans-serif;
    font-size: 16px;
    font-weight: 500;
    line-height: 21.6px;
    text-align: center;
    background-color: #fff;
    cursor: pointer;
    width: 65%;
    margin-left: auto;
    color: #000;
}


</style>