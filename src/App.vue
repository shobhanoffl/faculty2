<template>
  <v-app>
    <app-nav-bar />
    <span class="nav-title">
      Faculty
    </span>
    <v-main>
      <router-view/>
    </v-main>

  </v-app>
</template>

<script>
import AppNavBar from './components/AppNavBar.vue';

export default {
  name: 'App',
  components: {
    AppNavBar
  },
  data(){
    return{
      //
    }
  },
};
</script>

<style scoped>
.nav-title{
  text-align: center;
  width: 100%;
  margin-top: 23px;
  font-size: 26px;
  padding-bottom: 18px;
}
@media only screen and (max-width: 900px){
  .nav-title{
    text-align: center;
    width: 100%;
    margin-top: 23px;
    font-size: 26px;
    padding-bottom: 0px;
  }
}
</style>