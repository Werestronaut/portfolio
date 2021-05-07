<template>
  <div class="project">
<v-container>
  <v-row>
    <v-col cols="12">
        <div class="back" @click="$router.go(-1)">
          <i class="fas fa-sort-down fa-3x"></i>
          <h2>Tilbage til projekter</h2>
        </div>
    </v-col>
  </v-row>

</v-container>
    <v-container>
      <v-row>
        <v-col cols="12" align="center" justify="center">
          <div class="project-top">
            <div class="image-frame">
              <div class="image-box">
                <h3>Titel</h3>
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

.back:hover {
  right: 3em;
  i{
    color: #50a4ff;
  }
  h2{
    color: #50a4ff;
  }
  
}

.back {
  display:flex;
  flex-direction: row;
  align-items: center;
  transition: 300ms;
  right: 0em;
  position:relative;
  i{
    transform: rotate(90deg);
    color: #3A3A3A;
    transition: 300ms;
  }
  h2{
    font-size: 200%;
    line-height: 110%;
    font-family: halyard-display,sans-serif;
    font-weight: 600;
    font-style: normal;
    color: #3A3A3A;
    width: 25vw;
    transition: 300ms;
  }
}

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

    h3{
    font-size: 300%;
    line-height: 110%;
    font-family: halyard-display,sans-serif;
    font-weight: 600;
    font-style: normal;
    color: #3A3A3A;
    position: absolute;
    top: 40vh;
    right: 19vw;
    width: 50vh; 
    line-height: 80%;
    }
  }
}



</style>