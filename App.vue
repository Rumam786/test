<template>
  <div id="app">
    <h1>{{title}}</h1>
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <ruman />
    <ruman2 />
    <child v-on:changetitle="updatetitle($event)"/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import child from './components/child.vue'
import ruman from './components/ruman.vue'
import ruman2 from './components/ruman2.vue'
export default {
  name: 'App',
  components: {
    // HelloWorld,
    child,
    ruman,
    ruman2
  },
  data() {
    return {
      title: "props tutorial"
    }
  },
  methods: {
    updatetitle(title) {
      this.title=title
    }
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
