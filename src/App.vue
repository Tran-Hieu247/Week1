<template>
  <v-app>
      <BaseCardHeader></BaseCardHeader>
      <BaseCardBody></BaseCardBody>
      <BaseCardFooter></BaseCardFooter>
  </v-app>
</template>

<script>
  import BaseCardHeader from './components/views/BaseCardHeader.vue'
  import BaseCardBody from './components/views/BaseCardBody.vue'
  import BaseCardFooter from './components/views/BaseCardFooter.vue'
  export default {
    name: 'App',
    components:{
      BaseCardHeader,
      BaseCardBody,
      BaseCardFooter,
    }
    }
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  background-color: #ffffff;
  /* margin-top: 60px; */
}
.line{
  margin: 0 40px 0;
  height: 1px;
  width: calc(100%-80px);
  background: #0000001A;
}
</style>