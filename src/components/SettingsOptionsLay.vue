<template>
<!-- This component has Options (Settings) arranged vertically -->
  <div class="element-wrap">
      <div class="elements" v-for="option in optionnames" :key="option.icon">
          <v-icon color="black">{{option.icon}}</v-icon> 
          &nbsp;&nbsp;{{option.opname}}
      </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            optionnames: [
                {icon:'mdi-lock',opname:'Change Password'},
                {icon:'mdi-wallpaper',opname:'Display'},
                {icon:'mdi-account-cog',opname:'Others'}]
        }
    }
}
</script>

<style scoped>
/* Only Internal CSS */
.element-wrap{
    margin: 0 auto;
    width: 400px;
    background: white;
    margin-top: 100px;
}
.elements{
    padding: 10px;
    margin-bottom: 30px;
    text-align: left;
    /* border-left: 5px solid #3a7bd5; */
}
.elements:hover{
    background-color: rgba(2, 158, 247, 0.2);
    border-radius: 20px;
}

@media only screen and (max-width: 600px) {
  .element-wrap{
    width: 300px;
  }
}
</style>