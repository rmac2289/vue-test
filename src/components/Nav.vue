<template>
  <nav>
    <div v-on:click="alertMe">
      <a v-bind:href="url1">Portfolio</a>
      <a v-on:click="alertMe" href="">Alert!</a>
    </div>
  </nav>
</template>

<script>
export default {
  data: function() {
    return {
      url1: "https://www.ross-scott-macdonald.com",
    };
  },
  computed: {
    alertMe: function() {
      return alert("hey bud");
    },
  },
};
</script>

<style>
a {
  color: white;
}

nav {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 50px;
  position: fixed;
  background: #2c3e50;
  top: 0;
  left: 0;
  right: 0;
}
</style>
