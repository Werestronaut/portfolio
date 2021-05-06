<template>
  <div class="home">
    <v-row>
      <v-col cols="12"  class="lighten-5" id="front-text">
        <div class="home-text-container">
          <h3 class="text-right">{{dato}}</h3>
         
          <h4 class="text-right">Tag et kig rundt og se om du finder noget du kan lide</h4>    
        </div>
        <div class="home-image-self">
          <img src="../assets/sky.jpg" alt="">
        </div>
        <div class="outline-box">
          
        </div>  
        </v-col>
    </v-row>

  </div>
</template>

<style lang="scss" scoped>
.container {
  padding:0 !important;
}
.home{
  height: calc(100vh - 9em);
  overflow: hidden;
}
h3 {
  font-size: 420%;
  line-height: 110%;
  font-family: halyard-display,sans-serif;
  font-weight: 600;
  font-style: normal;
  color: #3A3A3A;
}

h4 {
  font-size: 390%;
  line-height: 110%;
  font-family: halyard-display, sans-serif; 
  font-weight: 300; 
  font-style: normal; 
  color: #3A3A3A;
}
#front-text {
  display: flex;
  flex-wrap: wrap;
  position:relative;
}
.home-text-container {
  width: 50%;
  margin: 2em 0 0 50px;
  z-index: 33;
     position: relative;
}

.home-image-self {
  width: 50%;
  height: 30%;
  margin: 0 0 0 -50px;
   z-index: 3;
   position: relative;
}

.outline-box{
  border: #333333 4px solid;
  width:50%;
  height:40%;
  position: relative;
  margin:-70px 0 0 200px;
  z-index: 1000;
}


</style>

<script>
export default {

  data() {
    return {
      dato: null
    }
  },

  mounted() {

      this.dato = `${new Date()}`;
      this.dato = this.dato.split(" ")[4].split(":")[0]


      if(this.dato > 6){
        this.dato = "God morgen!"
         
      }else if(this.dato > 12){
         this.dato = "God middag!"
      }else if(this.dato > 14){
      this.dato = "God eftermiddag!"
      }else if(this.dato >= 18){
         this.dato = "God aften!"
      }else{
        this.dato = "God nat!"
      } 
    //console.log(this.date)
      
      }
    
   
  
}
</script>
