<template>
  <menuPage/>
  <router-view/>
</template>

<script>
import menuPage from './views/menuPage.vue';
export default {
  name: 'App',
  components:{
    menuPage
  }
}
</script>

<style>
body{
  margin:0
}
</style>
