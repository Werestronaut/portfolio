<template>
  <div class="om-mig">
     <v-row>
      <v-col cols="12" md="4" offset="1">
        <div class="frame-clouds">
          <img src="../assets/sky_about.jpg" alt="">
          <div class="frame-outline">
            <div class="frame-self"></div>
          </div>
        </div>
        </v-col>
      <v-col  cols="12" sm="5" md="7">
        <div class="desc-text">
          <h3>Halløj, jeg hedder Markus</h3>
          <p>But I must explain to you how all this mistaken idea of denouncing pleasure and praising pain was born and I will give you 
a complete account of the system, and expound the actual teachings of the great explorer of the truth, the master-
builder of human happiness. No one rejects, dislikes, or avoids pleasure itself, because it is pleasure, but because those 
who do not know how to pursue pleasure rationally encounter consequences that are extremely painful. Nor again is 
there anyone who loves or pursues or desires to obtain pain of itself, because it is pain, but because occasionally 
circumstances occur in which toil and pain can procure him some great pleasure. To take a trivial example, which of us 
ever undertakes laborious physical exercise, except to obtain some advantage from it? But who has any right to find fault 
with a man who chooses to enjoy a pleasure that has no annoying consequences, or one who avoids a pain that 
produces no resultant pleasure?</p>
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

        <v-divider></v-divider>

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
      <div class="line"> </div>
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
  width: 50vw;
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
  width:468px;
  height:600px;
  .frame-outline{
    border: #333333 4px solid;
    position: absolute;
    width: 100%;
    height: 100%;
    top: 15px;
    left: 15px;
  }
}

.line {
  background-color: #333333;
  height: 5px;
  width: 40em;
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