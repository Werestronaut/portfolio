<template>
  <div class="om-mig">
     <v-row class="row">
      <v-col cols="6" md="4" sm="1" offset="1">
        <div class="frame-clouds">
          <img src="../assets/sky_about.jpg" alt="">
          <div class="frame-outline">
            <div class="frame-self"></div>
            <img src="../assets/Port_sitting.png" alt="">
          </div>
        </div>
        </v-col>
      <v-col  cols="4" md="2" sm="9" >
        <div class="desc-text">
          <h3>Halløj, jeg hedder Markus</h3>
          <p>Jeg er en 23-årig multimediedesigner der studere på EASV i Esbjerg, med passion og erfaring indenfor UX/UI-design og videoproduktion, da evnen til at skabe et detaljeret produkt falder mig naturligt.
                UX er en vigtig del af min design proces, da design ikke bare er noget der skal se godt ud, men skal fylde et formål.</p>
              <p>Jeg er en meget rolig og inkluderende person, der arbejder meget struktureret om det så skulle være gruppe eller solo arbejde.</p>
        </div>

        <div class="desc-bar">
            <div class="text-xs-center">
    <v-dialog
      v-model="dialog"
      width="600"
      height="355"
    >
      <template v-slot:activator="{ on }">
       <v-btn color="primary" elevation="3" rounded large v-on="on">Video CV</v-btn>
      </template>

      <v-card>
        <v-card-text>
           <iframe width="560" height="315" src="https://www.youtube.com/embed/dQw4w9WgXcQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 
        </v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn
            color="primary"
            flat
            @click="dialog = false"
          >
            Luk
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </div>
        </div>
        </v-col>
    </v-row>
    
  </div>
</template>

<style lang="scss" scoped>

/* .frame-clouds{
  width: 2em;
  height: 1em;
}

.frame-outline{
  border: #333333 4px solid;
  width:468px;
  height:600px;
  position: relative;
  margin: 0px 0 -615px 15px;
  z-index: 1000;
} */

.desc-text {
  width: 48vw;
  h3{
  font-size: 300%;
  line-height: 110%;
  font-family: halyard-display,sans-serif;
  font-weight: 600;
  font-style: normal;
  color: #3A3A3A;
  margin-bottom: 2vh;
  }
  p {
font-family: halyard-display, sans-serif; 
font-weight: 300; 
font-size: 120%;
font-style: normal; 
text-align: justify;
color: #3A3A3A;
margin-bottom: 5vh;
  }
}

.frame-clouds{
  position: relative;
  width:27.840571088637716vw; /* 468px */
  height:70.09345794392523vh; /* 600px */
  img{
    width:27.840571088637716vw;
  height:70.09345794392523vh;
  }
  .frame-outline{
    border: #333333 4px solid;
    position: absolute;
    width: 100%;
    height: 100%;
    top: 15px;
    left: 15px;
      .frame-self{
      position: absolute;
      left: 0vw;
      top: 0vh;
    }
    img{
      transform: translate(-19%, 3%);
      width: 44.49732302201071vw;  /* 748px */
      height: 110.98130841121495vh; /*950px*/
    }
  }

}

.row {
  overflow: hidden;
  padding-bottom: 11.7vh;
  
}
</style>

<script>
export default {
    data () {
      return {
        dialog: false
      }
    }
  }
</script>