<template>
  <div id="app">
    <p>style1:</p>
    <Step :now-step="nowStep" :step-list="stepList"></Step>
    <p>style2:</p>
    <Step :now-step="nowStep" :step-list="stepList" style-type="style2"></Step>
  </div>
</template>

<script>
import Step from "./components/Step.vue"

export default {
  name: "app",
  data() {
    return {
      nowStep: 2,
      stepList: ['First Step', 'Second Step', 'Third Step', 'Four Step']
    };
  },
  components: {
    Step
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
