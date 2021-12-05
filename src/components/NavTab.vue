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
    return{
      //
    }
  }
}
</script>

<style scoped>
/* Internal CSS Only */
#app .v-tabs{
	flex:0.1;
}
.main-tab{
  width: 700px;
  margin-left: auto;
  margin-right: auto;
  margin-top: 10px;
}

@media only screen and (max-width: 700px) {
  .main-tab{
    width: 600px;
  }
}

@media only screen and (max-width: 600px) {
  .main-tab{
    width: 100%;
  }
}
</style>