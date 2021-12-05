<template>
<!-- This Layout is the Default Template used to Show the Posts -->
  <div class="post-wrap">
    <div class="post-header">
        <img :src="postProfilePicURL" class="avator">

        <div class="post-header-info">
            <div class="post-header-line-one">
              <a class="location-link mintext"><v-icon small>mdi-map-marker</v-icon> {{postLocation}}</a>
              <span style="float:right;margin-right: 10px;" class="mintext">{{postMonth}} {{postYear}}</span>
            </div>
            &nbsp;<div style="margin-top:6px;margin-left:1px;display:inline-block;font-size:16px;">{{postProfileName}}</div> 
            &nbsp;·<span class="mintext"> Attended a {{postContent}}</span>
            <p class="post-caption">{{postCaption}}</p>
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
export default {
    data(){
        return{
            postLocation:'Erode',
            postProfilePicURL:'https://pbs.twimg.com/profile_images/1295112038096629760/3eCOaKDb_400x400.jpg',
            postFirstPicURL:'https://www.smartinsights.com/wp-content/uploads/2020/03/The-theory-of-Golden-Circle-model.png',
            postProfileName:'Simon Sinek',
            postMonth:'December',
            postYear:'2021',
            postContent:'Seminar',
            postCaption:'The Golden Circle theory explains how leaders can inspire cooperation, trust and change in a business based on his research into how the most successful organizations think, act and communicate if they start with why.',
            postImageNos:'2',
            postFistDocName:'The Golden Circle',
            postDocNos:'1'
        }
    }
}
</script>

<style scoped src="../assets/styles/post-lay.css">
/* There's a CSS File in src>assets>styles with Same File Name separated with Hyphens */

</style>