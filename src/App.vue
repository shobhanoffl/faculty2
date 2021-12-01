<template>
<AppNavBar iconList='iconList' />
</template>

<script>
// import HelloWorld from './components/HelloWorld';
import AppNavBar from './components/AppNavBar';

export default {
  name: 'App',

  components: {
    // HelloWorld,
    AppNavBar
  },

  data: () => ({
    iconList:['mdi-home','mdi-account','mdi-cog'], //AppNavBar for Main App
    tabs:["All","Posts","Seminars","Courses","Projects"] //NavTab for Main App
  }),
};
</script>