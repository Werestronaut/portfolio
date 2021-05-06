<template>
  <div class="project">
    <v-container>
      <v-row>
        <v-col cols="12" align="center" justify="center">
          <div class="project-top">
            <div class="image-frame">
              <div class="image-box">
              </div>
            </div>
          </div>
        </v-col>
    </v-row>
  </v-container>


  
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
#app{
  background-color: #F4F4F4 !important; 
}

.project-box{
    background-color: #884242; 
    width: 100%;
    height: 50%;
   // display:flex;
   // align-items: flex-start;
   // top: -20vh;

}

.image-frame{
  border: #333333 4px solid;
  width:600px;
  height:400px;

  .image-box{
    background-color: red;
    width: 100%;
    height: 100%;
    position: relative;
    top: -15px;
    left: -15px;
  }
}



</style>