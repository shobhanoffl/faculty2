<template>
<v-app>
    <v-tabs fixed-tabs scrollable show-arrows color="#3a7bd5" slider-size="2.5" class="main-tab">
        <v-tab @click="activeTab='Profile'">Profile</v-tab>
        <v-tab @click="activeTab='General'">General</v-tab>
        <!-- <v-tab @click="activeTab='FAQ'">FAQ</v-tab> -->
        <v-tab @click="activeTab='Contact Us'">Contact Us</v-tab>
  </v-tabs>
  <edit-profile-lay v-if="this.activeTab=='Profile'"/>
  <settings-options-lay v-else-if="this.activeTab=='General'"/>
  <contact-us v-else-if="this.activeTab=='Contact Us'"/>
  <!-- <f-a-q v-else-if="this.activeTab=='FAQ'"/> -->
</v-app>
</template>

<script>
import ContactUs from '../components/ContactUs.vue'
import EditProfileLay from '../components/EditProfileLay.vue'
// import FAQ from '../components/FAQ.vue'
import SettingsOptionsLay from '../components/SettingsOptionsLay.vue'
export default {
    name:'Settings',
    data(){
        return{
            activeTab:'Profile'
        }
    },
    components: {
        EditProfileLay,
        SettingsOptionsLay,
        ContactUs,
        // FAQ
    }
}
</script>

<style>
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