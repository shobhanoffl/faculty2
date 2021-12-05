<template>
<v-app>
    <profile-page-lay />
    <nav-tab :tablist="tablist" />
    <post-lay />
</v-app>
</template>

<script>
import ProfilePageLay from '../components/ProfilePageLay.vue'
import PostLay from '../components/PostLay.vue'
import NavTab from '../components/NavTab.vue'

export default {
    name: 'Profile',
    data(){
        return{
            tablist:['All','Posts','Seminars','Courses']
        }
    },
    components: {
        ProfilePageLay,PostLay,
        NavTab
    },
}
</script>

<style>
/* */
</style>