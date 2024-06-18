<template>
    <div class="view">
        <h3>OUR HAPPY CUSTOMERS</h3>
        <section>

            <cmt-custom v-for="data in data" :key="data" :data="data"></cmt-custom>
        </section>
    </div>
</template>

<script>
import CmtCustom from './CmtCustom.vue'
import cmt from '../../assets/cmt.json'
export default {
  components: { CmtCustom },
    component:{
        CmtCustom
    },
    data(){
        return {
            data: cmt
        }

    }
}
</script>

<style scoped>
section{
    display: flex;
    overflow-x: auto;
    max-width: 100%;
    gap: 20px;
}
h3{
    margin: 30px 0;
    font-family: Integral CF, sans-serif;
    letter-spacing: -.07em;
    font-size: 48px;
    font-weight: 800;
    line-height: 57.6px;
    text-align: center;
    margin-right: auto;
}
.view{
    display: grid;
    justify-items: center;
    padding: 0 100px;
    margin: 70px 0;
}
</style>