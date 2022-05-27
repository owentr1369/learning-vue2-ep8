<template>
  <div>
    <h1>UserComp</h1>
    <h2>My name : {{ customName }}</h2>
  </div>
</template>

<script>
export default {
  // Props dung de truyen du lieu tu cac comp cha sang comp con
  // va cac comp con tuyen thong bao den cac comp cha thong qua event
  props: {
    customName: {
      type: String,
      default: "Hello",
    },
  },
};
</script>

<style>
</style>