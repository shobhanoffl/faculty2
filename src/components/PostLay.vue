<template>
<!-- This Layout is the Default Template used to Show the Posts -->
  <div class="post-wrap">
    <div class="post-header">
        <img :src="postProfilePicURL" class="avator">

        <div class="post-header-info">
            <a class="location-link mintext"><v-icon small>mdi-map-marker</v-icon>{{postLocation}}</a>
            <span style="float:right;margin-right: 10px;" class="mintext">{{postMonth}} {{postYear}}</span>
            <br>
            &nbsp;<div style="margin-top:6px;margin-left:1px;display:inline-block;font-size:16px;">Steve Jobs</div> 
            &nbsp;·<span class="mintext"> Attended a {{postContent}}</span>
            <p>{{postCaption}}</p>
        </div>
    </div>
    <div class="align-straight">
      <img :src="postFirstPicURL" class="multi-img">
    </div>
    <span class="attached-link"> + {{postImageNos}} images</span><br>
    <div class="align-straight">
      <div class="document-wrap" style="display: inline-block;">
        <v-icon dense>mdi-file-document</v-icon> {{postFistDocName}} 
      </div>
      <div class="document-wrap" style="display: inline-block;">
        + {{postDocNos}} 
      </div>
    </div>
    <div class="align-straight like-bar">
      <span><v-icon>mdi-thumb-up</v-icon></span>
      <span style="float:right;margin-right: 20px;"><v-icon>mdi-bookmark</v-icon></span>
      </div>
  </div>
</template>

<script>
import "@/assets/styles/post-lay.css";
export default {
    data(){
        return{
            postLocation:'',
            postProfilePicURL:'',
            postFirstPicURL:'',
            postLocation:'',
            postMonth:'',
            postYear:'',
            postContent:'',
            postCaption:'',
            postImageNos:'',
            postFistDocName:'',
            postDocNos:''
        }
    }
}
</script>

<style scoped>
/* There's a CSS File in src>assets>styles with Same File Name separated with Hyphens */

</style>