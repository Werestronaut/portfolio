<template>

  <v-app>
    <header>
      <figure>
        <router-link to="/">
          <img src="./assets/hvidt_logo.svg" alt="logo" style="">
        </router-link>
      </figure>
      <div>
      <router-link to="/portfolio">Portfolio</router-link>
      <router-link to="/om-mig">Om mig</router-link>
      <router-link to="/kontakt">Kontakt</router-link>
      </div>
    </header>
     <v-main>
     <v-container id="dadum" fluid>
    <router-view>
    </router-view>
     </v-container>
   

    </v-main>
  </v-app>
</template>
<style>
  .container, .container--fluid {
  padding:0 !important;

}

</style>
<style scoped lang="scss">

img {
width: 17.84651992861392vw;
height:11.682242990654206vh;
}

header {
  margin-bottom: 3em;
  height: 6em;
  padding-right: 1.784651992861392vw;
  padding-top: 1.784651992861392vw;
  display: flex;
  align-items: center;
  justify-content: space-between;
  a{
    margin-right: 1.784651992861392vw;
    font-family: Helvetica, Arial, sans-serif;
    font-size: 125%;
    color: #707070;
    text-decoration: none;
    transition: 200ms;
  }
  a:hover {
    color: #50a4ff;
    text-decoration: none;
  }
}


</style>

<script>
/* import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
}; */
</script>
