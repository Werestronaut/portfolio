<template>
  <div class="kontakt">
    <v-container class="kontakt-container">
    <v-row class="kontakt-content" >
      <v-col cols="6" align="center" justify="center">
      <div class="kontakt-text">
        <h1>Lad os komme i kontakt</h1>
      </div>
      </v-col>

      <v-col cols="12" align="center" justify="center">
      <div class="outline-box">

        <div class="info-box">
          <h2>E-mail</h2>
          <a href="mailto:markus@hvidt.nu?subject=%F0%9F%91%8B%20Markus%20!%20">markus@hvidt.nu</a>
        </div>
        <div class="linkedin-box" href="https://www.linkedin.com/in/markus-hvidt-pedersen-01a85b205">
         <a href="https://www.linkedin.com/in/markus-hvidt-pedersen-01a85b205" style="width:60px; height:60px;" class="fab fa-linkedin fa-6x"></a>
        </div>
      </div>
      </v-col>
    </v-row>
    </v-container>
  </div>
</template>

<style lang="scss" scoped>

.kontakt-content{
  display: flex;
  justify-content: center;
}

.kontakt-text{
  h1{
    font-size: 300%;
    //line-height: 110%;
    font-family: halyard-display,sans-serif;
    font-weight: 600;
    font-style: normal;
    color: #3A3A3A;
   // margin-bottom: 2vh;
  } 
}

.info-box {
  background-color:#E6E6E6;
  position: relative;
  top: -1em;
  left: -1em;
  height:100%;
  width:64.666%;
  margin-right: 3%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  h2{
    font-size: 200%;
    line-height: 110%;
    font-family: halyard-display,sans-serif;
    font-weight: 600;
    font-style: normal;
    color: #3A3A3A;
    margin-bottom: 2vh;
  }

  a{
    font-family: halyard-display, sans-serif; 
    font-weight: 300; 
    font-size: 150%;
    font-style: normal; 
    color: #3A3A3A;
  }
}

.outline-box {
  border: #333333 4px solid;
  height: 140px;
  width: 456px;
  display: flex;
}

.linkedin-box {
  background-color:#E6E6E6;
  position: relative;
  top: -1em;
  left: -1em;
  width: 32.333%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;

  a{
    color:#333333;
    display: flex;
    align-items: center;
    justify-content: center;
    text-decoration: none;
  }
}
</style>