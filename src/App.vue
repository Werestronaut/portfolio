<template>

  <v-app>
    <header>
      <figure>
        <router-link to="/">
          <img src="./assets/logo.svg" alt="logo" style="width:300px; height:100px;">
        </router-link>
      </figure>
      <div>
      <router-link to="/portfolio">Portfolio</router-link>
      <router-link to="/om-mig">Om mig</router-link>
      <router-link to="/kontakt">Kontakt</router-link>
      </div>
    </header>
    <router-view>
    </router-view>
    <v-main>
      <HelloWorld/>
    </v-main>
  </v-app>
</template>

<style scoped lang="scss">

header {
  margin-right: 30px;
  margin-top: 30px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  a{
    margin-right: 30px;
    font-family: Helvetica, Arial, sans-serif;
    font-size: 20px;
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
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
