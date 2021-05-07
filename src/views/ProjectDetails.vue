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
                
                <h3>{{project.projectTitle}}</h3>
         
      
              <v-img :src="project.projectCover" alt="" />
              </div>
            </div>
          </div>
        </v-col>
      </v-row>
    </v-container>
    <v-container>
      <v-row justify="center" class="port-content">
        <v-col sm="6" md="8" lg="12">
        <div>
          <h2>1. Context & Problem statement</h2>
           <h3>{{project.projectContext}}</h3>
           
        </div>
        </v-col>
        <v-col sm="6" md="8" lg="12">
        <div>
          <h2>2. Løsning</h2>
           <h3>{{project.projectLosning}}</h3>
            <h4>{{project.projectLosTit}}</h4>
            <h3>{{project.projectLos2}}</h3>
            <h4>{{project.projectLosTit2}}</h4>
            <h3>{{project.projectLos3}}</h3>

        </div>
        </v-col>
        <v-col sm="6" md="8" lg="12">
        <div>
          <h2>{{project.projectResultatText}}</h2>
           <h3>{{project.projectResultat}}</h3>

           <div class="ResultImg">
           <v-img :src="project.projectResultatImg" alt="" max-width="15.2%" height="auto"/>
           <v-img :src="project.projectResultatImg2" alt="" max-width="36.5%" height="auto"/>
           </div>
        </div>
        </v-col>
      </v-row>
  </v-container>


  
  </div>
</template>

<script>
export default {
  
  data() {
    var project = this.$route.params
    return {
      project: {
        id: project.id,
        projectTitle: project.projectTitle,
        projectContext: project.projectContext,
        projectCover: project.projectCover,
        projectThumb: project.projectThumb,
        projectLøsning: project.projectLosning,
        projectResultat: project.projectResultat,
        projectLosTit: project.projectLosTit,
        projectLos2: project.projectLos2,
        projectLosTit2: project.projectLosTit2,
        projectLos3: project.projectLos3,
        projextResultatText: project.projectResultatText,
        projectResultatImg: project.projectResultatImg,
        projectResultatImg2: project.projectResultatImg2,
      }
    }
  },
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
  margin-bottom: 30px;
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
    /*background-image: ;*/
    width: 100%;
    height: 100%;
    position: relative;
    top: -15px;
    left: -15px;

    h3{
    font-size: 300%;
    line-height: 80%;
    font-family: halyard-display,sans-serif;
    font-weight: 600;
    font-style: normal;
    color: #3A3A3A;
    position: absolute;
    text-align: left;
    top: 36vh;
    left: 2vw;
    width: 62vh; 
    z-index: 100;
    }
  }
}

.port-content {
  margin-top: 30px;
  h3{
    font-family: halyard-display, sans-serif; 
    font-weight: 300; 
    font-size: 120%;
    font-style: normal; 
    text-align: justify;
    color: #3A3A3A;
  }

  h4 {
    font-family: halyard-display, sans-serif; 
    font-weight: 600; 
    font-size: 120%;
    font-style: normal; 
    text-align: justify;
    color: #3A3A3A;
    margin-top: 10px;
  }

  .ResultImg{
    margin-top: 30px;
    display:flex;
    flex-direction: row;
    justify-content: space-evenly;
  }
}


</style>