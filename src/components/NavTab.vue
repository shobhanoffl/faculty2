<template>
<!-- This component is a common Navigation Tab used in many places -->
  <v-tabs fixed-tabs scrollable show-arrows color="#3a7bd5" slider-size="2.5" class="main-tab">
    <v-tab v-for="tab in tablist" :key="tab">
      {{tab}}
    </v-tab>
  </v-tabs>
</template>

<script>
export default {
  props: ['tablist'],
  data(){
    //
  }
}
</script>

<style scoped>
/* Internal CSS Only */
#app .v-tabs{
	flex:0.1;
}
.main-tab{
  max-width: 55%;
  margin-left: auto;
  margin-right: auto;
  margin-top: 10px;
}
@media (max-width:961px){
  .main-tab{
    max-width: 100%;
  }
}
</style>