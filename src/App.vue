<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld />
    <UserComp v-bind:customName="myName" />
    <button @click="changeName">Change Name</button>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import UserComp from "./components/UserComp.vue";
export default {
  name: "App",
  components: { HelloWorld, UserComp },
  data() {
    return {
      customName: {
        type: Object,
        required: true,
        // Required = true phai co du lie, neu khong co se loi
        default: "Tam",
      },
    };
  },
  methods: {
    changeName() {
      this.myName = "Cmm";
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
