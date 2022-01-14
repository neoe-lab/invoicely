<template>
  <div id="wrapper">
    <h1>{{ username }}</h1>
    <p>{{ lastname }}</p>
    <a v-bind:href="links">Link</a>
    <h3>{{ getname() }}</h3>
    <!-- <p> Using mustaches : {{tac}} </p>
	<p>Using v-html directive : <span v-html="tac"></span></p>	 -->
  </div>
</template>
<script>
export default {
  name: "App",
  data() {
    return {
      username: "hello world",
      lastname: "LASTNAME",
      links: "https://www.google.com",
      // tac: "<span>TAG HTML</span>"
    };
  },
  methods: {
    getname() {
      return "HERO";
    },
  },
};
</script>
<style lang="scss">
@import "../node_modules/bulma";
</style>
