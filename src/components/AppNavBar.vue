<template>
<!-- This Component is the Floating Type Navigation Bar in Main App i.e., after login -->
  <div class="menu-component">
    <nav>
      <ul class="menu-bar">
        <li @click="toShow = !toShow"><v-icon color="black">mdi-menu</v-icon></li>
        <router-link to="/" class="nav-link">
        <li @click="toShow = false" :style="{display:[toShow ? 'Block' : 'None']}">
            <v-icon color="black">mdi-home</v-icon>
        </li>
        </router-link>
        <router-link to="/Profile" class="nav-link">
        <li @click="toShow = false" :style="{display:[toShow ? 'Block' : 'None']}">
            <v-icon color="black">mdi-account</v-icon>
        </li>
        </router-link>
        <router-link to="/Settings" class="nav-link">
        <li @click="toShow = false" :style="{display:[toShow ? 'Block' : 'None']}">
            <v-icon color="black">mdi-cog</v-icon>
        </li>
        </router-link>
      </ul>
    </nav>
  </div>
</template>

<script>
export default{
  data() {
    return{
      toShow : false
    }
  },
  methods(){
  }
}
</script>

<style scoped src="../assets/styles/app-nav-bar.css">
/* There's a CSS File in src>assets>styles with Same File Name separated with Hyphens */
</style>