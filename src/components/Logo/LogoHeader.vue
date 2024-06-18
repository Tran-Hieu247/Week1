<template>
    <div>
        {{logoName}}
    </div>
</template>
<script>
export default {
    props:{
        logoName: {
            type: String,
        }
    },
}
</script>

<style scoped>
    div{
        font-family: Integral CF, sans-serif;
        font-size: 32px;
        letter-spacing: -.09em;
        font-weight: 800;
        line-height: 38.4px;
        text-align: left;
        margin-right: 50px;
        cursor: pointer;
    }
</style>