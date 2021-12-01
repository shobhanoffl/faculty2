<template>
<!-- This Component is the Floating Type Navigation Bar in Main App i.e., after login -->
  <div class="menu-component">
    <nav>
      <ul class="menu-bar">
        <li @click="toShow = !toShow"><v-icon>mdi-menu</v-icon></li>
        <li v-for="icon in iconList" :key="icon" @click="toShow = false" :style="{display:[toShow ? 'Block' : 'None']}">
            <v-icon>{{icon}}</v-icon>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
import "@/assets/styles/app-nav-bar.css";
export default{
  data () {
    return{
        props:  ['iconList'],
        toShow : false
    }
  },
  methods(){
  }
}
</script>

<style scoped>
/* There's a CSS File in src>assets>styles with Same File Name separated with Hyphens */
</style>