<template>
    <div class="notify">
        <div class="msg-notify">
            Sign up and get 20% off to your first order.
            <a>Sign Up Now</a>
        </div>
        <v-btn class="xBtn" icon="mdi mdi-window-close" variant="text" color="white" size="20px"></v-btn>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
    .notify {
        width: 100%;
        height: 38px;
        background-color: #000;
        color: #fff;
        display: flex;
        justify-content: center;
        align-items: center;
        box-sizing: border-box;
        
    }
    .msg-notify{
        font-size: 14px;
        font-weight: 400;
        line-height: 18.9px;
        text-align: left;
        font-family: Satoshi, sans-serif;
    }
    a {
        text-decoration: underline;
    }

    .xBtn {
        position: absolute;
        right: 10%;
    }

    @media (max-width: 748px) {
        .notify {
            font-size: 12px;
            height: 34px;
        }
    }
</style>
