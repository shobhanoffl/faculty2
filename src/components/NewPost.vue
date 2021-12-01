<template>
<!-- This Component is used to Create New Posts -->
<div class="newpost-wrap">
  <v-form>
    <div class="newpost-title">What's up
      <span class="expand-icon" @click="expandBar=!expandBar"><v-icon color="#3d83e4">mdi-arrow-down-drop-circle-outline</v-icon></span>
    </div>
    <div class="expandable-part" v-if="expandBar">
      <br>
      <v-select label="Post Type" v-model="selectedPost" :items="postTypes" outlined></v-select>
      <v-textarea v-model="newPost" :counter="280" label="New Post" hint="Share your Achievement !" required outlined></v-textarea>
      <span class="update-link" @click="showAttach=!showAttach"><v-icon color="#3a7bd5">mdi-attachment</v-icon> Attach Files</span>
      <div class="newpost-icons" v-if="showAttach==true">
        <v-file-input  small-chips  multiple dense prepend-icon="mdi-wallpaper" accept="image/*" ></v-file-input>
        <v-file-input  small-chips  multiple dense prepend-icon="mdi-file-document" accept="document/pdf, document/docx"></v-file-input>
      </div>
      <div class="update-btn">Post</div>
    </div>
  </v-form>
</div>
</template>

<script>
export default {
  data:() => ({
    expandBar:false,
    showAttach:false,
    newPost:'',
    postType:null,
    selectedPost:'Usual',
    postTypes:['Seminar','Course','Project','Usual']
  })
}
</script>

<style scoped>
/* Only Internal CSS */
.newpost-title{
  font-size: 18px;
  font-weight: 500;
  color: rgb(34, 34, 34);
  margin: 2px auto 20px 3px;
}
.newpost-wrap{
  width: 55%;
  margin-top: 25px;
  padding: 25px;
  margin-right: auto;
  margin-left: auto;
  height: auto;
  border-radius: 25px;
  border: 1.5px solid rgba(0, 0, 0, 0.2);
}
.newpost-wrap:hover,.newpost-wrap:focus,.newpost-wrap:focus{
  border: 1.5px solid white;
  box-shadow: 1px 1px 8px 3px rgba(0, 0, 0, 0.2);
}
.newpost-icons{
  padding: 20px 0;
}
.update-link{
    color: #3a7bd5;
    text-align: center;
    padding: 2px;
    font-weight: 500;
}
.update-btn{
    background: #3d83e4;
    padding: 12px 25px;
    color: white;
    font-weight: 500;
    border-radius: 35px;
    border: 2px solid #3d83e4;
    text-align: center;
    margin-left: auto;
    margin-right: auto; 
    width:min-content;

}
.update-btn:hover{
    background-color: white;
    color: #3d83e4;
    border: 2px solid #3d83e4;
}
.expand-icon{
  float: right;
}
</style>