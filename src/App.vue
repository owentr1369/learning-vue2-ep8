<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld />
    <UserComp />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import UserComp from "./components/UserComp.vue";
export default {
  name: "App",
  components: { HelloWorld, UserComp },

  methods: {
    changeName() {
      this.name = "Cmm";
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
