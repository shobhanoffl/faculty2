<template>
<!-- This Component is used to to get feedback/suggestion from users -->
  <v-app class="contactus-wrap">
      <v-form>
          <h2>Contact Us</h2>
          <p>Thank You Visiting this Page...Kindly Reach us by writing your suggestion/critic/report/questions</p>
          <v-textarea v-model="contactus" :counter="500" label=" Contact Us " prepend-icon="mdi-message-draw" required outlined>
          </v-textarea>
          <br>
          <div class="update-btn">Send</div>
      </v-form>
  </v-app>
</template>

<script>
export default {
  data:() => ({
    contactus:''
  })
}
</script>

<style scoped>
/* Interal CSS Only */
.contactus-wrap{
    width: 700px;
    margin-right: auto;  
    margin-left: auto;  
    padding: 0 50px;
    margin-top: 60px;
}
.contactus-wrap h2{
    padding-bottom: 25px;
    text-align: center;
}
.contactus-wrap p{
    text-align: center;
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

@media only screen and (max-width: 700px) {
  .contactus-wrap{
    width: 600px;
  }
}

@media only screen and (max-width: 600px) {
  .contactus-wrap{
    width: 100%;
  }
}

</style>